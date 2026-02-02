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
* **Wrong County:** The signer is not registered in the same county as the county listed on the sheet.

The sections below first explain **what is acceptable or unacceptable by field**, because this is the easiest way to learn and memorize the rules. After that, you’ll find a summary section explaining **when to use each validity option**.

***

### Name Rules

#### First Name

First names are flexible.

* First names **can** be shortened or abbreviated, although **not** initialized.
* Common and reasonable nicknames are acceptable.

Examples:

* _Michael → Mike_
* _Elizabeth → Liz_
* _Derek → Der_

If everything else matches, this is still **Valid**.

#### Last Name

Last names are **not flexible**.

* Last names **cannot** be shortened, abbreviated, initialized, or otherwise altered.
* The written last name must match the voter database exactly.

There are two important exceptions:

**Double Last Names**

Some voters have two last names (often hyphenated or compound names).

* A voter with a double last name only needs to write **one** of their last names.
* This is still considered **Valid**, even though the written name differs from the database.

{% hint style="warning" %}
**Important warning about double last names in the database:**

Sometimes double last names appear in the voter database as a single word, without a space or hyphen. This is especially common with Spanish surnames.

Real Example:

* Signer writes last name: **Velez**
* Voter database shows last name: **Veleznavarro**

At first glance, this may look unusable. However, this is actually a **Valid** signature. Be on the lookout for these cases and take a moment to confirm whether the database last name is actually two names combined.
{% endhint %}

**Married Name Changes**

If a signer writes a married last name but is still listed in the database under their original last name (or vice versa), this must be marked as a **Failed Match**.

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

Street names can be flexible, but not vague.

* Street names may be **reasonably** shortened, abbreviated, or contain minor spelling errors and still be **Valid**.
* Street names **cannot** be fully initialized.

Example of unacceptable initialization:

* _10 LB St_ for _10 Long Beach St_

This could mean multiple different streets and cannot be reliably interpreted.

**Multi-Word Street Names**

For streets with multiple words:

* Writing only the first word is acceptable.
* Shortening one or both words is acceptable.
* Initializing **all** words is not acceptable and should be marked as a **Failed Match**.

#### Address Mismatch Scenarios

If the signer’s name matches one or more voter records, but the address and/or city does not align, this is generally a **Failed Match**.

Even if you think beyond a reasonable doubt that the signer is a certain voter record due to their unique or rare name but the address doesn't match (a soft match), you need to mark these as a **Failed Match**.

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

Either the city **or** the ZIP code may be incorrect — but **not both**.

Valid scenarios:

* City incorrect, ZIP correct → **Valid**
* ZIP incorrect, city correct → **Valid**

Invalid scenario:

* City incorrect **and** ZIP incorrect → **Failed Match**
* Either the city or zip are missing

***

### County Rules

Each petition sheet includes a county line, which is spliced out and presented to you.

* Every voter on the sheet **must be registered in that county**.
* If you find a voter match from a different county, do **not** validate it.

This is **Wrong Town**.

Always double-check county alignment manually.

***

### Other Disqualifying Conditions

The following always result in **Unusable** signatures:

* Not every field is filled out
* Any field is crossed out
* The signature appears black-striped or covered in Sharpie
  * These were disqualified before upload — delete them using the red trash can button

***

### Validity Summary (How to Categorize)

#### 🟢 Valid

* Signature meets CA rules
* Voter is selected
* Minor, acceptable discrepancies only
* If all required information is present but simply on the wrong lines, still valid&#x20;

#### 🟠 Failed Match

* Signature is at least partially readable and all fields are present
* Information does not match voter database
* Includes:
  * No voter found
  * Address mismatch
  * Married name mismatch
  * Both city and ZIP incorrect
  * First name is initialized (_T. Brogan)_

#### 🔴 Unusable

* Signature is structurally disqualified or totally illegible
* Includes:
  * Last name is abbreviated, shortened, or initialized
  * Missing street number
  * PO Box
  * Blank fields
  * Crossed-out fields
  * Wrong county

{% hint style="warning" %}
**On illegible signatures**

If a signature is **legible&#x20;**_**enough**_ that you can attempt to make a search, no matter how small, but you can't find it, it's Failed Match

If a signature is **so illegible** that you can't even attempt to make a search, it's Unusable
{% endhint %}

#### 🟡 Wrong County

* Signer is not registered in the same county as the county listed on the sheet
* Quickly compare the county of a potential match to the county written on the sheet
* If the county of the voter does not match the written county, mark the signature as **Wrong County**

{% hint style="warning" %}
Some petitions have a backside, or multiple pages. The county is typically written on the first or front page only.

For backsides or sheets without a county written on them, validate signatures without considering the county.&#x20;
{% endhint %}

***

### Important Edge Cases

<figure><img src=".gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

**🔴 Unusable** — The last name appears to be shortened.

***

<figure><img src=".gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

**🔴 Unusable** — The last name is omitted.

<figure><img src=".gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

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

🟢 **Valid** — Signer wrote one of their two last names, which is Valid.

<figure><img src=".gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

***

<figure><img src=".gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

:x: **Delete —** Black-striped signatures should be deleted, not marked as Failed.&#x20;

***

### Final Reminder

Learn what is acceptable **by field first**.

Once you know that, the correct validity option becomes obvious

If something is readable but mismatched → **Failed Match**\
If something is structurally wrong → **Unusable**\
If the signer's county does not match the written county → **Wrong County**\
If everything lines up → **Valid**

Consistency matters more than speed.
