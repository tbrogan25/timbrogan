---
description: This document explains how to apply California validity rules in Certifi.
---

# CA Validity Rules

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

![](.gitbook/assets/image.png)
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

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

If you don't see a splice for the county, find it by looking at the full sheet on the right.

If there's no county, select NO COUNTY.

#### Signature County

If you mark a signature as Failed Match, you will be prompted to enter the signer's city or zip code.

This is so we can determine what county the signer is from on our end.

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

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

### Soft- and Strict-Searching

If you can't find a signature using the strict search or if it's too illegible for you to gather enough information to use the strict search, toggle on the soft search.&#x20;

The soft search requires less accuracy, so minor spelling errors are allowed (although not too many).

{% hint style="danger" %}
Always use the soft search if you can't find a voter with the strict search.
{% endhint %}

<figure><img src=".gitbook/assets/image (189).png" alt=""><figcaption><p>Soft search is on</p></figcaption></figure>

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
