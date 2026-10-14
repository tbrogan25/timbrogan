---
hidden: true
---

# Learning Certifi: Week 2

10/14/26

I have already set up Certifi locally on my laptop and was able to login to an admin account I created. I encountered some bugs but used ChatGPT to help me get over them. The next day, I started up Certifi with `npm run dev:up` and noticed the self-hosted admin panel was perpetually loading, but with a Certifi loading icon and custom white background. The backend was up but one ingredient wasn't working.&#x20;

I run `npm run dev:status` to see if any services are down and the docker service `certifi-mongo` was not marked "healthy" but "health: starting", which was a symptom of the error yesterday. I realized then that it was the same error happening again and recurring for some reason. I had to stop it permanently.

To temporarily fix the problem and get Mongo working for now, I used the same commands I learned when the issue was happening yesterday. They stop the entire service, delete the volume containing the old container name, and rebuild the volume with the new correct container name.

```
docker inspect certifi-mongo --format '{{range .Mounts}}{{println .Name "->" .Destination}}{{end}}'
npm stop
docker volume rm certifi-app_mongo-data
npm start
```

I used ChatGPT to help me troubleshoot and I gave it some log output. We found that the Docker container that holds the Mongo database was named after the Docker container's temporary ID, so everytime the container was rebuilt for some reason (which happens automatically in the background), the Mongo container's name would change too. The original name gets stored in the corresponding volume (persistent storage unlike the actual container), and then the newly-renamed container can't communicate with the volume due to the name mismatch.

To fix this, I needed to edit one of the docker compose files, `docker-compose.local.yml` and add a custom hostname to the container, which I named `mongo`

<figure><img src=".gitbook/assets/image (230).png" alt=""><figcaption></figcaption></figure>

Because I had deleted the volume earlier, I needed to re-add my admin email to the list of allowed emails:

`ADMIN_EMAIL=powersbrogantechnologies@gmail.com ./scripts/create-admin.sh`

The Mongo issue had been fixed permanently.&#x20;

Now I want to be able to use Git to start saving versions of my own local Certifi. This is because I intend to make my own features during my learning process and will want to keep track of all the versions of "my" Certifi that exist after each feature I add. This will also be useful in the event that I brick my local Certifi and need to go back to a previous version.
