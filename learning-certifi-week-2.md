---
hidden: true
---

# Learning Certifi: Week 2

10/14/26

I have already set up Certifi locally on my laptop and was able to login to an admin account I created. I encountered some bugs but used ChatGPT to help me get over them. The next day, I started up Certifi with `npm run dev:up` and noticed the self-hosted admin panel was perpetually loading, but with a Certifi loading icon and custom white background. The backend was up but one ingredient wasn't working.&#x20;

I run `npm run dev:status` to see if any services are down and the docker service `certifi-mongo` was not marked "healthy" but "health: starting", which was a symptom of the error yesterday. I realized then that it was the same error happening again and recurring for some reason. I had to stop it permanently.

To temporarily fix the problem and get Mongo working for now, I used the same commands I learned when the issue was happening yesterday. They stop the entire local Certifi server, delete the volume containing the old container name, and rebuild the volume with the new correct container name.

```
docker inspect certifi-mongo --format '{{range .Mounts}}{{println .Name "->" .Destination}}{{end}}'
npm stop
docker volume rm certifi-app_mongo-data
npm start
```

I used ChatGPT to help me troubleshoot and I gave it some log output. We found that the Docker container that holds the Mongo database was named after the Docker container's temporary ID, so everytime the container was rebuilt for some reason (which happens automatically in the background), the Mongo container's name would change too. The original name gets stored in the corresponding volume which does NOT get randomly recreated like the container, and then the newly-renamed container can't communicate with the volume due to the name mismatch.

To fix this, I needed to edit one of the docker compose files, `docker-compose.local.yml` and add a custom hostname to the container, which I named `mongo`

<figure><img src=".gitbook/assets/image (230).png" alt=""><figcaption></figcaption></figure>

Because I had deleted the volume earlier, I needed to re-add my admin email to the list of allowed emails:

`ADMIN_EMAIL=powersbrogantechnologies@gmail.com ./scripts/create-admin.sh`

The Mongo issue had been fixed permanently.&#x20;



**10/15**

Now I want to be able to use Git to start saving versions of my own local Certifi. This is because I intend to make my own features during my learning process and will want to keep track of all the versions of "my" Certifi that exist after each feature I add. This will also be useful in the event that I brick my local Certifi and need to go back to a previous version without losing all of my work up until that point.

```
# makes new branch
git switch -c tim-learning

# switches branch
git switch tim-learning

# shows the status of my edits
git status

# shows the edits i made in the files
git diff

# prepares my edits to be committed
git add .

# commits my changes
git commit -m ""

# See all commits & their messages
git log
```

<figure><img src=".gitbook/assets/image (231).png" alt=""><figcaption></figcaption></figure>

I successfully committed all my changes, but now I need to create a repository outside of my local machine.

In the browser, I created a new private repo in Bitbucket called `certifi-tim-sandbox` so my work would be separate from the real Certifi code. Then I used the following commands to push my new branch to this Bitbucket repository:

```
# Add my new Bitbucket repo as a new external repo that my local machine knows
git remote add sandbox git@bitbucket.org:pbt-workspace/certifi-tim-sandbox.git
```

"Sandbox" is the local nickname for the external Bitbucket repo actually named "certifi-tim-sandbox"

```
# Show all remote repositories that my local Git repo knows about
git remote -v
```

"sandbox" will show up in this now.

"origin" is the default nickname made by Git for the repo that I initially cloned from. So "origin" is the equivalent of "sandbox" but for Elizabeth's official Certifi repository

<figure><img src=".gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

Next I need to push my local version of Certifi that includes my committed edits to this external repo

```
git push -u sandbox tim-learning
```

`-u` tells Git to remember the subsequent pairing of the remote repo (sandbox) and the branch (tim-learning) so I no longer need to worry about pushing my changes in the tim-learning branch to the origin repo

Going forward, I only need to type `git push` whenever I want to push my changes to my sandbox repo

<figure><img src=".gitbook/assets/image (234).png" alt=""><figcaption></figcaption></figure>

Now all my changes are in my own private sandbox repo! This version of Certifi can be pulled down from the Internet now!
