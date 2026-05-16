---
layout: post
title:  "Phish Has a Bimmer"
author: mainphish
tags:
  - content
  - phish
  - badphish
  - email
  - subscription
  - service
categories: 
  - blog
---

This phishing email is a variation of the one that claims you bought 
something -- usually a subscription -- and gives you a way to contact the
phisher to cancel said subscription, and get phished in the process. 
The difference is that instead of starting it, it is warning that
it is ending/cancelling said subscription. 

In this case, the subscription is for something related to 
[Bimmer World](https://www.bimmerworld.com/), a website selling parts for,
as you guessed, BMW cars. As far as I know, the only subscription they
have is for their (spammy) 
[news feed](https://www.bimmerworld.com/About-Us/E-News-Signup/).
So, the email could be claiming to be talking about that, or that you have
not bought enough junk so they are closing the account. 
Now go take a quick look at the email and be the judge; we will 
get back after you read it and will then talk about it.

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: Mon, 27 April 2026 19:18:55 +0000
From: Data Protection Team <support@bimmerworld.com>
Subject: Failed: Subscription Terminated
To: Clueless Phish <cluelessphish@phishphillet.com>

Failed: Subscription Terminated
Cloud Storage
! Scheduled for Deletion

Dear User,

This is a notification regarding the data hosted on your inactive account. 
Per our retention policy, files on inactive accounts are scheduled for 
permanent removal on .
Status: Pending Deletion
Photos: 4,203 files found
Videos: 112 files found
Action: Renew to prevent loss
[Keep My Files]

If you allow your account to expire, we cannot recover your files once 
they are deleted from our servers.

[Unsubscribe]

</pre>

`[Keep My Files]` and `[Unsubscribe]` are the same link because, well, this is 
a phishing expedition.

## Why this looks like phishing to me 

Let's eliminate the obvious one: that perhaps neither of us have ever
bought anything from that site. Let's assume that we are not really sure
or this game will end too quickly.

The phisher had a great opportunity to make the phishing email believeable, 
but lost it. Allow me to show you how that was done.

- The email claims a tons of videos and photos (i.e. media) will be removed. 
If this is supposed to be for an account you buy junk from, or receive
junk email from, it should not have a ton of media that it implies you 
uploaded. That would only make sense if this was a forum or a site like 
icloud or photobucket. 

- The email mentioned some *cloud storage*, which would support what was
said in the previous bulletpoint: icloud, google drive/photos, photobucket,
and dropbox would all fit that. 
Even any online car, if wanting to use that theme, forum would work, would
give that required suspension of belief any good phishing email needs.
The phisher raised my expectations, but as 
you will see next, he/she crushed them expertly.

- *Bimmer World*! What does that have to do with cloud storage? 
Nothing, absolutely nothing. 

I am disappointed, even insulted. 
I have seen, and posted here, phishing emails that are so bad they
are entertaining; this is not one of them.


## We need your help!

I try to post samples of good, bad, and weird phishing messages here but I 
can only do so much on my own. I need your help! If you receive a 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">phishing message</a> </b>
-- email, text, or even voicemail, and want me to tear it apart and
make fun of it, send 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">the phishing message</a> </b>
to us so we can phillet it for you!

