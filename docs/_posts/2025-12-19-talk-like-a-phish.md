---
layout: post
title:  "Talk Like a Phish"
author: mainphish
tags:
  - content
  - phish
  - notdphish
  - email
categories: 
  - blog
---

We have cover here many examples of phishing emails, showing how to identify
them. 
We also talked about the reasons they work: 
they are crafted just enough to make potential victims wonder if they are 
real so they will click on a link or attachment, or even call the 
phisher. The sense of urgency in these messages make said victims take those
actions before stopping and thinking if the email is legitimate. 
There is, however, another reason: some of those phishing emails are dead
copies of real, legitimate emails. Case in point is today's message, which
I myself have received on Saturday.
And, it has most of the items would make me think "that is a honest-to-goodness
phishing email!" Let's take a look at it and how *yours truly* handled it.

So I shipped a package through [UPS](https://www.ups.com) on Nov 24. On
Nov 27, it reached the first UPS location... and has not moved from said
location since according to tracking info. After a *month* (yeah, shame on
me for procrasinating so much), I contacted them, creating a case. 
A week after case was created, I got an email with instructions to file
a claim for the value of the package + shipping. And then I received the
following email:

**Note:** yes, I do have a gmail account which I use to receive such messagesr. I also
have other email accounts; my work email is not through gmail for many reasons
I would rather not talk about here or I would be writing until next week.

<img src="/images/2025/stop-it-help.png"
class="align-center" alt="[Screen capture of the suspicious email whose text version is shown below]">

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: Sat, 13 Dec 2025 00:19:58 -0500
From: <no-reply@upscapital.com>
Message-ID: <8889997654.abba.1234567890abc@QWERTYUIO.us.ups.com>
Subject: UPS Capital Claims document for ClaimNumber: 000-06-123456
To: Clueless Phish <cluelessphish@gmail.com>

To Whom It May Concern,

Please review the attached.

If you have any questions, please contact me directly.

Regards,
UPS Capital Insurance Agency, Inc. - 2C47342
Claims Representative
 One attachment --¢  Scanned by Gmai

[Attachment]

</pre>

Attatchement is a pdf, one of the classic file types used to hide malicious
code, and is called 
`000-06-123456_WWEConfirmationOfPayment_12122025_181053.pdf` 
(claim number + `WWEConfirmationOfPayment` + date.pdf).

## Why this looks like phishing to me 

- Why is the return address `upscapital.com` instead of `ups.com`?

- `To Whom It May Concern`? I have seen more suspicious emails with much less
vague salutation. 

- `Please review the attached.` I would not be surprised if I either have
posted a phishing email with these very words here. 
This is the classical "*I have an important message to you but you will have
to open my malicious attachment to find out what so I can infect your computer
or scare you into contacting me so I can get your personal info*" kind of
phishing email.
If you are legit, use your words! 
Can't you tell me why you are contacting me and what should I expect to see 
in the email?

- `If you have any questions, please contact me directly.` Contact who?
There is no name or real contact info in the email.
The return address is `no-reply@upscapital.com` which means if you reply to
the email they will cheerfully ignore you.
Once again, it is expected that I will open the pdf attachment where
*all will be made clear*, i.e. the classical phishing email I mentioned
right on the previous bullet point.

- `Scanned by Gmail`. Is that supposed to make me feel comfortable?
It is not that hard to craft a malicious email attachment which will pass
the gmail scanners with flying colours.

## Well, what are you going to do about it?

Now that I vented about it, had some nice warm relaxing tea, and took a deep
breath (no knee-jerk reaction!), I can do some researching:

- *Do I have any notes or docs about this claim?* Actually I do, and the claim
   number listed (`000-06-123456`) does match a screen capture I did when 
   I fille out the claim. Bottom line, *always keep docs of 
   contracts/purchases/claims/etc you so so you can verify against that*.

- *Do I have other ways to verify the claim status?* Yes I do as I have the
  url to the claims portal website. And that I did, using the additional info
  from previous bullet. In there I found the name and email of the claim 
  adjuster,
  the result of the claim, and there is a PDF in that page whose name is
  exactly what was in the email. I will download it and compare the two files
  (for the techies around you, I will use `sha256 checksum`).

- *What if I did not have access to the claims site?* I would call UPS's
  support line and stay there until they connect me to someone with a clue.
  For instance, does UPS own "UPS Capital"?

- *What else did you do?* Well, I do have access to tools (I think by now you
  would expect nothing less) to inspect PDF files
  and see if they have malicious code. I used them in the file and found
  nothing. But not everyone has such tools.
  And I have not opened said pdf yet.

In the end, this was a legit email. Do I feel like a fool for spending so much
time researching it? Not at all: first I was doing the same procedure we keep
asking everyone to do: 

1. Slow down
1. Don't click on any links or download any attachments.
1. Does the email make sense?
1. Did you expect an email like that?
1. Do you have a way to verify the source? Who send this to you? By verifying I mean contacting who the email claims to come from using their official contact info, not what is in the email.

Second, they are going to send a check (no, I do not volunteer to connect my
bank account to any company out there. Really. Bad. Idea). So, if my claim
was approved, I will see the check in my mailbox. I can wait for that!

Third, if I am to autopilot, I would rather do these steps all the time even
if it delays acting on a legit email a bit.  AI is great but keeping your mind
sharp to identify phishing emails is better.
