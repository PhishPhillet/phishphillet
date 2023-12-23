---
layout: post
title:  "Facebook Phishing"
author: mainphish
tags:
  - content
  - phish
categories: 
  - blog
---

Yet another lazy phisher. The email supposedly pretends to be from facebook.
If you are like me and use a mail app that shows you the header and allows you
to see what the links in the email are really linking to, this email is 
just too obviously phishy. Unfortunately there are mail apps that act like 
the messaging ones
I mentioned before, not letting you find out what the button links to until
it is too late. I despise said programs with passion. 

Let's see if, in spite of that, we can smell this phishy email out:

<pre>
From: FB <niyupsevog@gmx.net>
reply-to: Facebook Datacenter <notification-fb@internet.ru>,
Facebook Datacenter USA1 <datacenterusa@list.ru>,
Facebook Datacenter USA2 <datacenterusa@internet.ru>,
Facebook Datacenter USA3 <datacenterusa@inbox.ru>,
Facebook Datacenter19 <datacenterusa@bk.ru>,
[...]
elgrandepe.supra007@icloud.com,
vaccard.ziyous@icloud.com,
fabino.malsbe07@yahoo.com,
savinmeanv@gmx.net,
tenerrunis@gmx.net,
tekeom@gmx.net,
akilxarqi49@mail.com,
aerkoulared50@mail.com,
inbox.boite@gmx.de
Date: 24 Nov 2023 11:23 AM
Subject: Someone tried to log into your account | ID# 87885
To: Clueless Phish <cluelessphish@example.com>

[Facebook Logo] 

Hi cluelessphish

A user just logged into your Facebook account from a new device: (Samsung Galaxy smartphone) Location: Vietnam, Pleiku, Province de Gia Lai
We are sending you this email to verify it's really you.

'If you are not the user, please click on "Report the user".

`[Report the user] [Yes, me]`

Thanks,
The Facebook Team

</pre>

## Identifying this phishing email
Let's see what we can do if we have an arm and tow legs tied behind our leg
because we chose to use a privacy-avert mail client:

- Even if we did not see the email address in the `From:` field (I would think
Facebook can afford an email in their own domain), I do not think it would be
called `FB`. Maybe *Customer Service* or *Abuse* would be better names even
if Facebook does not officially use them; they give a better official business
feel to the email than `FB`.
- I never received such email from Facebook; I guess it would require me to
have a facebook account to begin with. But, I checked a few and the look 
(even though I only pasted a text-only version) looks close enough. 
*What should you do then?* Well, **always login directly to their website**
and see if there is such a warning there. Don't click on buttons just 
because they look nice. Go to the official source and check there.
If you do not see a message, contact them.
- Why should the button to report a potential breach be called 
`[Report the user]`? Is that really how Facebook writes it? If so, I
would just do what I suggested in the previous bullet point.
- The line beginning with `'If you are not the user,` does not have a
single quote ending the one it started with. Small thing but once I saw it I 
could not take my eyes off it.

### If you can see links and header... it is even easier!
This time our mail client is a bit more helpful!

- That `Reply-to:` field seems to have everything and everyone listed in it.
Forget the Russian domains, that field should contain *one single email*, 
period. More than one is suspicious. More than ten? Stop being so obvious!
- If you hover over the `[Report the user]` you will see if you click on it, it
will create an email addressed to? You guessed right! Everyone listed in the
`Reply-to:` field we talked about. Mr Lazy Phisher, this is beyond careless!

As you can see, while sometimes you may be limited by mail apps which are way
too friend for their own good, a bit of attention may be enough to unmask
these more carelessly *crafted* (using the term loosely here) phishing emails.
