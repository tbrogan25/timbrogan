# MA Validity Rules

Validation is straightforward.&#x20;

There are two types of validation: Match & Search

### Match

Match validation is where you'll compare a signature to a pre-made validation decision.

The all-caps bolded text above the signature image is the validation decision.&#x20;

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Your job is to compare this decision to the actual signature image and determine if they match.

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

You also need to compare the town/city decision to the written town/city, which appears only once at the bottom of each page.

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

In the above example, they do match.

Here's another example:

<figure><img src=".gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

The signer wrote across the dividing line; this doesn't matter. As long as the core information matches, it's a match.

{% hint style="info" %}
**Core information:**

* First name
* Last name
* Street number
* Street name
* Town/city
{% endhint %}

Comfortably ignore middle names, apartment numbers, zip codes, street endings (St., Ln., Ave.), etc. They do not need to match.

The core information does not need to match the pre-made validation decision exactly.&#x20;

Spelling errors, initializations (T. Brogan instead of Timothy Brogan), out-of-order information (street THEN name), are all allowed.

Here's one last example:

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

This is a match, despite the messy and undecipherable last name. Everything else lines up.

Just remember this:

{% hint style="info" %}
If you can reasonably decide that the signer is the voter, _you can validate it_.

If there are parts of the signature that tell you it is NOT a match, do not validate it.
{% endhint %}

The signer's last name missing a letter here, but it's still a match:

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

This is an example of a non-match.

The last names, street names, and most obviously, the town names don't match.

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
To indicate a match: press V

To indicate a non-match: press X
{% endhint %}

### Search

Search validation is where you'll search for a signature that does not have a pre-made validation decision.

The town/city is located above the signature image.

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Your job is to find the signer from the database, and if they're not there, then you must mark it as the correct invalidity reason.

Here's an example of a typical signature:

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

Here's what you might search:

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

#### Search Order

The searchbar reads your search **left to right** in this exact order:

1. First Name
2. Last Name
3. Street Number
4. Street Name
5. City
6. Zip code

Each space separates one field.

**Always use this order. Do not deviate from it.**

#### Minimum Characters Per Field

When you enter a value for a field, you must type **at least two characters** for Certifi to search it.

One character is **not enough,** except for the street number.

**Rule of thumb:** If you only know one character, **skip the field.**

***

#### Skipping a Field

If you want to **skip a field entirely**, type a single period:

```
.
```

This tells Certifi: **“Ignore this field and move to the next one.”**

Here's an example

```
mary . 79 . attleboro
```

* First name is **"mary"**
* Last name is skipped
* Street number is **"79"**
* Street name is skipped
* City name is **"attleboro"**

<figure><img src=".gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

The signer was found! They are the second entry.

#### Searching Strategy

Search for whatever is clearest first.

This is usually the address (because people usually sign their names and print their address).

<figure><img src=".gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

The above example has a very clear address, allowing you to find the voter (second result).

<figure><img src=".gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

If **even one character is wrong,** it can completely prevent the correct voter from appearing.

The more characters you type, the more likely you are to misinterpret one and prevent the correct match from appearing at all.

For this reason, you should **always start with what is very clearly written**, using only the characters you are most confident about. If you get no results, remove a few characters and search looser again.

Once results appear, **then** tighten the search by adding more characters to narrow them down — never the other way around.

{% hint style="danger" %}
A loose search that returns results is **always better** than a precise search that returns nothing.
{% endhint %}

Many missed matches happen not because the voter isn’t in the database, but because **too much information was typed too early**.

However, if you still can't find a signer after loosening then tightening your search, you must use the _"_&#x53;oft search."

#### Soft Search

The "strict search" is the normal search you've learned about this whole time.

The "soft search" is meant to be more forgiving of cases where the spelling in your search query is just a little bit off.

Click this button and you'll know the soft search is activated when the searchbar becomes blue.

<figure><img src=".gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

It allows you to find a higher rate of valid signatures that you couldn't find with the strict search.

{% hint style="danger" %}
Use the soft search only after you've used the strict search at least twice, and failed.&#x20;
{% endhint %}

Do not rely on it to understand your guesses. One too many spelling errors, and it will fail to find your voter. It will not always find your misspelled searches.

Here's an example where it works:

<figure><img src=".gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

Let's say you search the following:

```
sara . 40 cedar aron
```

<figure><img src=".gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Nothing appears.&#x20;

Then, you toggle on the soft search.

<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

It worked!&#x20;

I was unknowingly misspelling the town as "aron" when it was "avon."

Here's another example:

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

```
patrick . 158 rowan bridge
```

<figure><img src=".gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

Nothing. Let's try the soft search:

<figure><img src=".gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

It worked!&#x20;

The signer's messy handwriting made the streetname hard to search for.

Remember to always try the strict search first followed by the soft search if you still can't find the voter.

### Examples

#### Valid

The following signature is very messy, but still matchable. Here's how I found it:

<figure><img src=".gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

```
. . 45 illian bridgewater
```

<figure><img src=".gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

The last result is the match!

This next one is also messy but matchable:

<figure><img src=".gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

```
debra . 49 . brockton
```

<figure><img src=".gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

The top result is the match!

This next one can still be matched despite the first name being initialized by the signer.

Remember:

**If you can reasonably decide that the signer is the voter,&#x20;**_**you can validate it**_**.**

This means initials are allowed if no one else at the address has that unique initial + last name combination.

<figure><img src=".gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

```
. . 810 precinct taunton
```

<figure><img src=".gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

#### Invalid

This next signature is missing two of the **core pieces of information:** the street number and street name.

<figure><img src=".gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

You can't match it to anybody. So, you'll mark it **Failed Match**.

Click on the signature image so it's highlighted blue, and press **"a"** on your keyboard.

You will also mark any signatures **Failed Match** if you cannot find them in the database.

There are two invalidity options: **Failed Match** and **Wrong Town**.&#x20;

**Wrong Town**

The town/city that the voter is registered to vote must be the same as the town written on the bottom of the sheet.

If it is not, you must mark the signatures as **Wrong Town** by clicking on the signature image and pressing **"d"** on your keyboard.

{% hint style="warning" %}
**NOTE: BEWARE OF "VILLAGES"**
{% endhint %}

There are a lot of "villages" in MA, which are neighborhoods of real cities/towns.

This is a problem because if a village name is written in the Town/City box and you use it in your searches, then none of the signatures on that sheet will appear!

If the written town on the bottom of the sheet differs from the town of the signer, refer to this link to make sure the written town is not a village! Villages are on the left, followed by the real town name.

[https://www.sec.state.ma.us/divisions/cis/historical/archaic-names.htm](https://www.sec.state.ma.us/divisions/cis/historical/archaic-names.htm)

#### Deleting Signatures

Sometimes you may need to click the red trashcan icon to delete signatures that shouldn't be validated at all.

The first of two examples is when a signature is fully crossed out.

These cannot be validated. They were crossed out so they would not be considered. Please delete them.

<figure><img src=".gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

The second example is when a row doesn't actually have a signature in it, or has only a half of an attempted signature. These aren't meant to be validated. Please delete these as well.

<figure><img src=".gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

### Pay

* Search: 5 cents/sig
* Match valids: 2 cents/sig
* Match invalids: 4 cents/sig
