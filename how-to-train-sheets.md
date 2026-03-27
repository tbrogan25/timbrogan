# How to Train Sheets

## Setting Up

Look at the pinned messages in #sheet-training

There, you can download the Sheet Labeler application

There, you will also see the state, project names, and number of sheets per each project that you should train.

Select the state

<figure><img src=".gitbook/assets/image (205).png" alt=""><figcaption></figcaption></figure>

Select the necessary project > Open Project

<figure><img src=".gitbook/assets/image (206).png" alt=""><figcaption></figcaption></figure>

On the left-hand side at the top, all of the turn-ins for this project are listed. Each turn-in is a group of petition sheets submitted by one petitioner for the selected project.&#x20;

You will need to download a turn-in before you can train the sheets that are in them.

1. Select multiple turn-ins and downloading them all by holding down Ctrl/Command and clicking multiple

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

The number of sheets in each turn-in are visible to the right, and the individual sheets are visible at the bottom (in this selected turn-in, 2 sheets).

<figure><img src=".gitbook/assets/image (207).png" alt=""><figcaption></figcaption></figure>

Once you've downloaded a turn-in, the sheets become available for you to train.&#x20;

Click on one at the bottom. The sheet will appear in the center of your screen.

<figure><img src=".gitbook/assets/image (208).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (209).png" alt=""><figcaption></figcaption></figure>

#### Blackstripes

30 of your 75 sheets should have contain a blackstriped row on it. This is crucial so we can train the splicing AI to navigate sheets that contain them.

Here's how to tell:

After downloading a lot of turn-ins for your given project, you can filter for sheets that contain blackstripes by clicking the corresponding icon, which is the red square, at the top.&#x20;

Then, simply click on 30 of these sheets and train them!&#x20;

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
A minority of the sheets labeled with a red square may not actually have a blackstripe on them. Make sure to train 30 sheets that actually have a blackstripe on them.
{% endhint %}

#### Recent Files First

We want to train the most recently uploaded scans because that quality is consistent with what will get uploaded over the remainder of the project.

The most recent files are at the bottom of the list of turn-ins. Please download these first and begin training these ones.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## Controls

* Zoom by scrolling up or down
* Drag the sheet around by holding down right-click (step 1), or holding down the scroll wheel (step 2)

## Video Example

{% embed url="https://www.youtube.com/watch?v=iUFXb7gPQO8" %}

## Step 1: Label Corners

First, we need to label the four corners of the big signature box to _fully encompass_ the border lines, excluding the columns on the left and right, like highlighted below. Remember, _we need to include the outer lines of the box itself._

The goal is to place the points on each corner so that the border lines are fully included in the splice, not excluded.

Below is the box I'm talking about.

<figure><img src=".gitbook/assets/image (211).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Your work needs to be exact. You must be incredibly detail-oriented with these tasks. Any wrong move will give the sheet-training AI the wrong information, which will create more splicing errors.
{% endhint %}

You will need to click on the exact point that is _just outside of the corner_.

Use the crosspoint at the top right to accurately place the pin.

For example, I would click the following point for the **top left corner** like this:

<figure><img src=".gitbook/assets/image (216).png" alt=""><figcaption></figcaption></figure>

This edited screenshot might help you understand what I mean:

<figure><img src=".gitbook/assets/image (217).png" alt=""><figcaption></figcaption></figure>

Notice how the pin would just barely encompass both border lines that converge at that corner.



Go in this order:

Top Left -> Top Right -> Bottom Right -> Bottom Left

Click Undo if you want to undo the last corner you labeled.&#x20;

Click Clear Step if you want to undo all corners you added.

Click Confirm Step when you're done.

## Step 2: Label Lines

Next, we need to label the horizontal lines within the big signature box, including the top and bottom lines of the big signature box.

You will know you did Step 1 correctly if you can see the four border lines. If not, please redo Step 1 by clicking on another sheet then clicking back on the sheet.&#x20;

You need to plot at least two points for each horizontal line.

Make your first point at the leftmost part of each line.

<figure><img src=".gitbook/assets/image (218).png" alt=""><figcaption></figcaption></figure>

Use the crosspoint at the top right again to make sure the horizontal crosspoints line up in the center of the line

<figure><img src=".gitbook/assets/image (219).png" alt=""><figcaption></figcaption></figure>

Some horizontal lines will be curved because these petitions were photographed, not scanned.

For curved lines, please plot as many points as necessary to replicate the curve.&#x20;

This is crucial, so we can train curved sheets to be spliced too. Curved sheets are the biggest culprit behind splicing errors.

Some lines will be straight, though. You can tell when you plot the second point at the rightmost part of the line. Your line will replicate the line exactly.

Press space to commit each line. It will turn yellow.

In the below example, I placed a point at the leftmost part of the line. But the line has curved upwards on the right side of the sheet.&#x20;

<figure><img src=".gitbook/assets/image (220).png" alt=""><figcaption></figcaption></figure>

This is where I'll place another point to replicate the line.

<figure><img src=".gitbook/assets/image (221).png" alt=""><figcaption></figcaption></figure>

Much better.&#x20;

Below is a video of me replicating the horizontal lines of a sheet:

{% embed url="https://youtu.be/08pURiXPU5Y" %}

## Step 3: Splice the County Box

Lastly, we need to splice the county box to tell the sheet-training AI where to make that splice.

This is the easiest step.

Left-click and drag your box to slightly include the top, bottom, and right lines of the box (if there is a box), and go as far as the words "vote in" on the left.

<figure><img src=".gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

If there is no box or the words are different, just make an equivalent sized box.

Clicking Confirm Step, then Save in the top right will bring you to the next sheet.

## Sending your results

We'll discuss getting the results from you this weekend!
