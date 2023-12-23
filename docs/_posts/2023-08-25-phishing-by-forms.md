---
layout: post
title:  "Phishing by Forms"
author: mainphish
tags:
  - content
  - phish
  - image
categories: 
  - blog
---
Google/Microsoft Office365 docs, forms included, are a great way to phish
someone. You create a document with a macro or just a link, and send it in a
way to entice the potential victim. We have talked about using the carrot
angle -- prizes and free money -- and the stick one -- fines and receipts
for outstanding bills -- but how about nothing at all? 
That is what this phisher is going for: no clever titles or descriptions, 
and no explanation for why you should fill the form.
All it offers is just a request, 
"*I've invited you to fill out the following form:*"

<img src="/images/2023/phish19.png" 
class="align-center" alt="[Phishing email with nothing else but a Google
form to be clicked on]">


Someone will be curious enough click on it.

<pre>
Reply-To: ali38@guru.sd.belajar.id
X-GoogleForms-FormId: **ID for suspicious Google form**
X-GoogleForms-CustomerDisplayName: Kementerian Pendidikan dan Kebudayaan Indonesia (SD)
Date: Sun, 20 Aug 2023 02:15:13 +0000
Subject: kjyhg
From: ali38@guru.sd.belajar.id
To: Clueless Phish <cluelessphish@example.com>

I've invited you to fill out the following form:
kjyhg

To fill it out, visit:
[** Link to suspicious Google form **]


Google Forms: Create and analyze surveys.

</pre>

## Identifying this as a phishing email

The basic test always start with "stop and think." If you spend more than
10s looking at this email, you may still be curious but your finger will no
longer be itching to click on the link:.

- The `Subject:` line is a dead giveaway, unless you expect emails from your cat.
- The `From:` field also shows the phisher is just not bothering to be subtle.
- The `X-GoogleForms-CustomerDisplayName:` field, which is usually not shown, is
interesting. Does that mean phisher was trying to impersonate the Indonesian
Ministry of Education and Culture?
If so, why didn't he put their logo in the body of the email?
Even if their name is in the form, that would take until opening said form to
see that, which would waste the reason to have that veneer of credibility.

There is nothing else I can say because, well, there is nothing else in this 
extremely lazy phishing email.
Do you think this phisher had a quota to fill and was just in a hurry?
