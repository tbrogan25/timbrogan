---
description: This document explains how to apply California validity rules in Certifi.
---

# CA Validity Rules

Validation is straightforward.&#x20;

There are two types of validation: Match & Search

### Match

Match validation is where you'll compare a signature to a pre-made validation decision.

The all-caps bolded text above the signature image is the validation decision.&#x20;

<figure><img src=".gitbook/assets/image (192).png" alt=""><figcaption></figcaption></figure>

Your job is to compare this decision to the actual signature image and determine if they match.

<figure><img src=".gitbook/assets/image (193).png" alt=""><figcaption></figcaption></figure>

You do not need to compare the county decision to the written county on the sheet. You can ignore this. If they don't match, it's fine.

<figure><img src=".gitbook/assets/image (194).png" alt=""><figcaption></figcaption></figure>

As long as the core information matches, it's a match.

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

Spelling errors, additional information, and out-of-order information (street THEN name), are all allowed, as long as the core information is present.

{% hint style="info" %}
To indicate a match: press V

To indicate a non-match: press X
{% endhint %}

### Search

Search validation is where you'll search for a signature that does not have a pre-made validation decision.

The county will be located above the signature image.

<figure><img src=".gitbook/assets/image (195).png" alt=""><figcaption></figcaption></figure>

Your job is to find the signer from the database, and if they're not there, then you must mark it as the correct invalidity reason.

Here's an example of a typical signature:

<figure><img src=".gitbook/assets/image (196).png" alt=""><figcaption></figcaption></figure>

Here's what you might search:

<figure><img src=".gitbook/assets/image (197).png" alt=""><figcaption></figcaption></figure>

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
. illi 15230 parth
```

* First name is skipped
* Last name contains **"illi"**
* Street number contains **"15230"**
* Street name contains **"parth"**

<figure><img src=".gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>

The signer was found! They are the first and only entry.

#### Searching Strategy

Search for whatever is clearest first.

This is usually the address (because people usually sign their names and print their address).

<figure><img src=".gitbook/assets/image (200).png" alt=""><figcaption></figcaption></figure>

The above example has a very clear address, allowing you to find the voter (second result).

<figure><img src=".gitbook/assets/image (201).png" alt=""><figcaption></figcaption></figure>

If **even one character is wrong,** it can completely prevent the correct voter from appearing.

The more characters you type, the more likely you are to misinterpret one and prevent the correct match from appearing at all.

For this reason, you should **always start with what is very clearly written**, using only the characters you are most confident about. If you get no results, remove a few characters and search looser again.

Once results appear, **then** tighten the search by adding more characters to narrow them down — never the other way around.

{% hint style="danger" %}
A loose search that returns results is **always better** than a precise search that returns nothing.
{% endhint %}

Many missed matches happen not because the voter isn’t in the database, but because **too much information was typed too early**.

However, if you still can't find a signer after loosening then tightening your search, you must use the _"_&#x53;oft search."

### Soft- and Strict-Searching

If you can't find a signature using the strict search or if it's too illegible for you to gather enough information to use the strict search, toggle on the soft search.&#x20;

The "strict search" is the normal search you've learned about this whole time.

The "soft search" is meant to be more forgiving of cases where the spelling in your search query is just a little bit off.

Click this button and you'll know the soft search is activated when the searchbar becomes blue.

<figure><img src=".gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

It allows you to find a higher rate of valid signatures that you couldn't find with the strict search.

The soft search requires less accuracy, so minor spelling errors are allowed (although not too many).

{% hint style="danger" %}
Always use the soft search if you can't find a voter with the strict search.
{% endhint %}

Do not rely on it to understand your guesses. One too many spelling errors, and it will fail to find your voter. It will not always find your misspelled searches.

Here's an example where it works:

<figure><img src=".gitbook/assets/image (202).png" alt=""><figcaption></figcaption></figure>

Let's say you search the following:

```
doris volpen 15149
```

<figure><img src=".gitbook/assets/image (203).png" alt=""><figcaption></figcaption></figure>

Nothing appears.&#x20;

Then, you toggle on the soft search.

<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (204).png" alt=""><figcaption></figcaption></figure>

It worked!&#x20;

I was unknowingly misspelling her last name as "volpen" when it was "volper"

Remember to always try the strict search first followed by the soft search if you still can't find the voter.

### Validity Options

You will work with the following validity outcomes:

* **Valid**
* **Failed Match:** The signature is readable and properly formatted but the  \
  signer is not registered to vote with the information they provided.
* **Unusable:** The signature is not readable or not properly formatted,  \
  regardless of whether the signer is registered to vote or not.

The sections below first explain **what is acceptable or unacceptable by field**, because this is the easiest way to learn and memorize the rules. After that, you’ll find a summary section explaining **when to use each validity option**.

***

### Name Rules

#### First Name

First names are flexible.

* First names **can** be shortened or abbreviated, although **not** initialized.
* Common and reasonable nicknames are acceptable.

Examples of valid nicknames and shortenings:

* _Michael → Mike_
* _Elizabeth → Liz_
* _Derek → Der_

If everything else matches, this is still **Valid**.

Examples of invalid initializations:

* _Tim Brogan → T Brogan_
* _Brendan James Powers → BJ Powers_

These are **Unusable**.

<figure><img src=".gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

#### Last Name

Last names are **not as flexible**.

They **cannot** be majorly shortened, abbreviated, or initialized.

There are three important exceptions:

**Messiness/Misspellings**

If a last name is messy and looks like it's missing a few letters, this can still be valid.

If a last name is misspelled or missing a minor amount of letters, this can still be valid.

**Double Last Names**

Some voters have two last names (often hyphenated or compound names).

* A voter with a double last name only needs to write **one** of their last names.
* This is still considered **Valid**, even though the written name differs from the database.

{% hint style="warning" %}
**Important warning about double last names in the database:**

Sometimes double last names appear in the voter database as a single word, without a space or hyphen. This is especially common with Spanish surnames.

Real Example:

* Signer writes last name: SMITH
* Voter database shows last name: **SMITHTILLERY**

At first glance, this may look unusable. However, this is actually a **Valid** signature. Be on the lookout for these cases and take a moment to confirm whether the database last name is actually two names combined.

![](<.gitbook/assets/image (2).png>)
{% endhint %}

**Married Name Changes**

If a signer writes a married last name but is still listed in the database under their original last name (or vice versa), this must be marked as a **Failed Match**. The information does not match.

***

### Street Address Rules

When reviewing addresses, **only focus on two things**:

* The **street number**
* The **main street name**

Ignore everything else.

#### What to Ignore

The following should always be ignored, even if they differ from the database:

* Apartment or unit numbers
* House fraction numbers (e.g., _10 1/2 Main St_)
* Directional prefixes (East, West, North, South)
* Street types (St, Ave, Cir, Blvd, etc.)

#### Street Numbers

* A street number **must be present**.
* The street number must match the database **exactly** to be Valid.

Outcomes:

* Incorrect street number → **Failed Match**
* Missing street number → **Unusable**

#### Street Names

* A street number **must be present**.
* Street names may be shortened, abbreviated, or contain minor spelling errors and still be **Valid**.

**Multi-Word Street Names**

For streets with multiple words:

* Writing only the first word is acceptable.
* Shortening one or both words is acceptable.

Outcomes:

* Missing street name → **Unusable**

#### PO Boxes

If a PO Box or other non-address information appears in the address field, the signature must be marked as **Unusable**.

***

### City & Zip Rules

#### City Names

City rules in California are **very lenient**.

* Cities may be shortened, abbreviated, or contain spelling errors.
* Cities may be initialized, even if they contain multiple words.
* Any abbreviation is acceptable (e.g., _LB = Long Beach_).
* If a city has multiple words, at least one letter per word is enough.

#### City and ZIP Interaction

Either the city **or** the ZIP code may be incorrect or missing — but **not both**.

Valid scenarios:

* City incorrect, ZIP correct → **Valid**
* ZIP incorrect, city correct → **Valid**
* City missing, ZIP correct → **Valid**
* ZIP missing, city correct → **Valid**

Invalid scenario:

* City incorrect **and** ZIP incorrect → **Failed Match**
* City missing **and** ZIP incorrect  → **Failed Match**
* ZIP missing **and** city incorrect → **Failed Match**
* City missing **and** ZIP missing → **Unusable**

***

### County Rules

#### Sheet County

Each petition sheet includes a county line, where the county is written by the signature-gatherer. Sometimes this will be spliced out and presented to you, sometimes not.

You must tag the county of the sheet in the COUNTY dropdown in the top left.

This only needs to be done once per sheet and you will be prompted to do so if it isn't filled out.

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

If you don't see a splice for the county, find it by looking at the full sheet on the right.

If there's no county, select NO COUNTY.

#### Signature County

If you mark a signature as Failed Match, you will be prompted to enter the signer's city or zip code.

This is so we can determine what county the signer is from on our end.

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Select the correct city/zip code and click Submit.

<figure><img src=".gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure>

***

### Mismatched Fields

If all of the necessary information is present but some fields are just swapped, the signature is still valid.

<figure><img src=".gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

***

### Blank Fields

If any fields are blank but the necessary information is squeezed in elsewhere, the signature is still valid.

<figure><img src=".gitbook/assets/image (185).png" alt=""><figcaption><p>City and zip are on the address line, "SF 94122"</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (184).png" alt=""><figcaption><p>City and zip are on the address line</p></figcaption></figure>

If the information is _not_ squeezed in elsewhere, it is **Unusable**.

***

### Blank Rows

Delete these using the red trash can icon. They were likely unintentionally captured during processing.

<figure><img src=".gitbook/assets/image (190).png" alt=""><figcaption></figcaption></figure>

***

### Blackstriped Signatures

If the signature appears black-striped or covered in Sharpie, the client did this and wants us to disregard this.&#x20;

These were disqualified before upload — delete them using the red trash can button.

<figure><img src=".gitbook/assets/image (186).png" alt=""><figcaption></figcaption></figure>

***

### Crossed Out Fields

Signatures where one or more (but not all) fields are crossed out are **Unusable**&#x20;

This is the equivalent of the street number and name being missing

<figure><img src=".gitbook/assets/image (181).png" alt=""><figcaption><p>Unusable</p></figcaption></figure>

Signatures where _all_ fields or the entire box are crossed out should be **deleted**

<figure><img src=".gitbook/assets/image (182).png" alt=""><figcaption><p>Delete</p></figcaption></figure>

We want to delete signatures that are **clearly marked for deletion by the petitioner themselves** before being sent to us.

This is the same reason why we delete **blackstriped signatures**: they are clearly marked for deletion to ensure that we do not consider them.

But for signatures where only one or more fields are crossed out, _but other parts of the signature are still present_, it is not marked for deletion; the signature-gatherer still submitted it to us.

***

### Validity Summary (How to Categorize)

#### 🟢 Valid

* Signature meets CA rules
* Voter is present in the database
* If all required information is present but simply on the wrong lines, still valid&#x20;
* If fields are blank but the necessary information is squeezed in elsewhere, still valid

#### 🟠 Failed Match

* Signature is at least partially readable and all fields are present
* Information simply does not match voter database
* Includes:
  * No voter found&#x20;
  * Married name mismatch
  * Both city and ZIP are incorrect

#### 🔴 Unusable

* Signature is structurally disqualified or totally illegible
* Includes:
  * First name is initialized (_T. Brogan)_
  * Last name is majorly abbreviated, shortened, or initialized
  * Missing information like signature, printed name, street number, street name, and both city and zip
  * PO Box in address
  * Crossed-out fields that _do not_ have the necessary information rewritten somewhere
  * Blank fields that _do not_ have the necessary information rewritten somewhere

***

### Important Edge Cases

<figure><img src=".gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

**🔴 Unusable** — The last name appears to be initialized.

***

<figure><img src=".gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

**🔴 Unusable** — The last name is omitted.

***

<figure><img src=".gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

🟢 **Valid** — Street directionals can be ignored, so this signature is Valid despite the missing "E" (East) prefix in the voter database.

***

<figure><img src=".gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

🟢 **Valid** — Cities can be abbreviated.

***

<figure><img src=".gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (163).png" alt=""><figcaption></figcaption></figure>

🟢 **Valid** — Cities can be abbreviated.&#x20;

***

<figure><img src=".gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

🟢 **Valid** — Signer wrote one of their two last names, which is Valid.

***

<figure><img src=".gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

:x: **Delete —** Black-striped signatures should be deleted, not marked as Failed.&#x20;

***

### Final Reminder

Learn what is acceptable **by field first**.

Once you know that, the correct validity option becomes obvious

If something is readable but not in the database → **Failed Match**\
If something is structurally wrong → **Unusable**\
If everything lines up → **Valid**

Consistency matters more than speed.

Good luck everyone!

\~ Tim B

### Pay

* Search: 12 cents/sig
* Match valids: 2 cents/sig
* Match invalids: 4 cents/sig
