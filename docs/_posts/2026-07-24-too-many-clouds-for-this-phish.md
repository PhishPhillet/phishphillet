---
layout: post
title:  "Too Many Clouds for this Phish"
author: mainphish
tags:
  - content
  - phish
  - copyphish
  - email
  - subscription
  - service
categories: 
  - blog
---

Sometimes I wonder if some phishers are plain lazy or there are seasons in
phishing. Case in point is that recently I have been receiving -- both
in some of my email accounts (google is always a guilty party) and from
those people who graciously submit phishing emails -- a lot of emails about
online storage subscriptions expiring.

Here is the one *I* received:

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: 23 Jul 2026 17:07:23 +0200 (CEST)
From: Cloud Management <support@chaosandpain.com>
Subject: Action needed within 24 hours to avoid losing backup capabilities.
To: Clueless Phish <cluelessphish@phishphillet.com>

Cloud Services

!
Storage Almost Full
Action needed to prevent sync disruption

Your 50 GB Storage Plan is at 98% capacity. Once full, your device will no 
longer back up photos, save new files, or receive incoming emails.

49.2 GB Used 50 GB Total
Recommended Plan 200 GB Premium
Exclusive Offer: 50% off your first 3 months
[Upgrade to 200 GB Storage]
Secure your files and continue syncing your photos seamlessly. This promotional upgrade offer expires in 24 hours.

Sent by Cloud Services Inc.
4563 Cloud Way, Server City, CA.

[Unsubscribe]
</pre>

And here is the one I received from a reader:

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: 23 Jul 2026 17:02:00 +0200 (CEST)
From: Account Care <support@flashresultats.fr>
Subject: Your cloud is almost full. Upgrade to 200 GB and keep your memories safe.
To: Clueless Phish <cluelessphish@phishphillet.com>

Cloud Services

!
Storage Almost Full
Action needed to prevent sync disruption

Your 50 GB Storage Plan is at 98% capacity. Once full, your device will no 
longer back up photos, save new files, or receive incoming emails.

49.2 GB Used 50 GB Total
Recommended Plan 200 GB Premium
Exclusive Offer: 50% off your first 3 months
[Upgrade to 200 GB Storage]
Secure your files and continue syncing your photos seamlessly. This promotional upgrade offer expires in 24 hours.

Sent by Cloud Services Inc.
4563 Cloud Way, Server City, CA.

[Unsubscribe]
</pre>

Separated at birth? If that is the case, this next one is a close cousin. At
least it offered more disks space (250 GB vs 50GB)

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: 23 Jul 2026 17:02:00 +0200 (CEST)
From: Account Care <support@flashresultats.fr>
Subject: Your cloud is almost full. Upgrade to 200 GB and keep your memories safe.
To: Clueless Phish <cluelessphish@phishphillet.com>

Cloud Services

!
Subscription Expired

Your 250 GB Storage Plan has expired and automatic renewal was 
not successful.

Plan 250 GB Cloud Storage
Status Inactive
Total Due $2.99
[Renew Subscription]
To prevent data loss, please update your billing information. 
Inactive accounts may be subject to deletion after 30 days. 

Sent by Cloud Services Inc.
4563 Cloud Way, Server City, CA.

[Unsubscribe]
</pre>

## Why I think these phishing emails are, well, you know

- Let's not beat around the bush: two emails, sent to two different people,
using two different return addresses but otherwise the same emails. 
If that is not suspicious I do not know what is.
The third one was also close enough to make me go "*now wait a minute!*"

The other clues would work even if you only saw one of them:

- They all pretend to be the same mythical generic "Cloud Services Inc."
in equally mythical "Server City" which of couse is in California. 
Nothing suspicious here... nope... not at all.

- The classic `From:` email address that has nothing to do with the mythical
company they pretend to be. Come on, that is low effort phishing.

- What is that exclamation mark doing all by itself? We will never know...

- Finally, the pressure to make the reader (or phish) to act before thinking.
Oh no! We have only 24h hours to act before doom! Doom! DOOOM!

These are not the only similar emails I gathered this week; I picked 
three of them ortherwise this post would be needlessly long.
But, this is what backs my initial question: "is this the season of *expiring
storage subscription* phishing emails?" 
As of now I have no idea, but if you do, please contact us!


## We need your help!

I try to post samples of good, bad, and weird phishing messages here but I 
can only do so much on my own. I need your help! If you receive a 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">phishing message</a> </b>
-- email, text, or even voicemail, and want me to tear it apart and
make fun of it, send 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">the phishing message</a> </b>
to us so we can phillet it for you!

