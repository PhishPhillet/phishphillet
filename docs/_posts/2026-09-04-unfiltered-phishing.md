---
layout: post
title:  "Unfiltered Phish"
author: mainphish
tags:
  - content
  - phish
  - filter
  - email
  - spam
categories: 
  - blog
---

Catching a phishing email is not a "*press the Ez-Button*" solution, even if you
press the "*AI Button*" no matter what vendors offer you. It is done better 
in layers:

- Filter spoofed emails. These are tests that do not care about the
   content of the email but focus on what we call the email header, which tells
   (or claims to tell) where the email came from. The idea here is to 
   verify that this email came from where it claims to.
- Filter emails that are coming from addresses and domains known to be used 
   to send malicious emails. These lists are known as "*Domain Name System 
   blocklists*" (DNSBL) and have been around since the late 1990s.
- Filter emails that have known telltale indicators for phishing/spam 
   emails. Now we are talking about looking inside the content of the email
   itself for suspicious patterns. I know this sounds like what we have been
   doing here at the [PhishPhillet](https://phishphillet.com/), but this is
   the kind of filtering that can be done with software, including AI.
- Filter emails that have attachments our email software detected as
   containing malware. 
- Filter emails that end user -- the potential phish -- looked at it and 
   thought it was suspicious. This is the one we created this website primarily
   to talk about, and our last line of defense.

These layers are placed in an increasing order of effort.
We hope that more of the phishing emails were caught by the (automated) steps 
so we only have to spend our (human) mind looking at a small set that felt 
through.

<img src="/images/2026/EZ_Button-sm.png"
class="align-center" alt="Picture (I took and badly cropped the background out) of an EZ/Easy Button">

In this case, we should expect our hope to expertly crushed.

Let's start with the low handing fruit, the spoof email filtering. Some of the
phishing emails we made fun of here claim to be from a real business 
such as [Venmo](https://phishphillet.com/blog/2023/07/07/phisher-goes-to-venmo.html),
but uses a `gmail` or some other email address they own

<pre style="white-space: pre-wrap; font-family: monospace;">
From: Venmo <venmopayunit123@gmail.com>
</pre>

which we can see has nothing to do with, in this case, Venmo. 
Others are real email addresses (for some reason they are fixated on the
support email addresses) from real companies like this one taken from 
a [recent post](https://phishphillet.com/blog/2026/07/24/too-many-clouds-for-this-phish.html):

<pre style="white-space: pre-wrap; font-family: monospace;">
From: Cloud Management <support@chaosandpain.com>
</pre>

This second case would be a classic case of spoof email filtering, and there 
the tools to detect it have been around since 2010. And you can see that in 
action by looking at the email header:

<pre style="white-space: pre-wrap; font-family: monospace;">
Authentication-Results: my.mail.server (dis=spam; info=dmarc default policy);
	dmarc=fail (dis=spam p=quarantine; aspf=r; adkim=r; pSrc=config) 
header.from=chaospain.com
</pre>

What the above mean is that my mail server took a look at that email
pretending to come from `Cloud Management <support@chaosandpain.com>` and 
found out that is a lie, that it did not come from `chaosandpain.com`'s mail
server, and is probably spam. Yes, it is that easy. You need to configure
your own business to authenticate your own mail server with your business, but
that is a couple of lines.

## So why you are talking about crushed hopes and spending so much time on this?

If you looked at our recent posts, you will see a lot of them have email 
addresses following the format `support@real.email.com` just like the 
`support@chaosandpain.com` we mentioned. I even have one for `support@yahoo.com`which is is a spam email pushing Alzheimer stuff.
Each of these emails should have been caught by a decent spoof email filter.
It turned out that gmail, microsoft, yahoo. and other email providers which I
expected to be filtering, or allowing we the users to filter, such emails
based on the `dmarc=fail` alert, are gladly putting these emails in the inbox.

I talked to some people I know and they are seen an explosion of spam and 
phishing emails with `From: support@real.email.com` headers.
Why they are not being caught? They are low hanging fruits.
Blindly blocking `support@real.email.com` means you may lose a legitimate email
from that address.

## What does that mean to us?

- Phishers and spammers found an oldie but still goodie way to pass their
  emails to us, unfiltered.
- There are more emails we have to deal with now.

## We need your help!

I try to post samples of good, bad, and weird phishing messages here but I 
can only do so much on my own. I need your help! If you receive a 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">phishing message</a> </b>
-- email, text, or even voicemail, and want me to tear it apart and
make fun of it, send 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">the phishing message</a> </b>
to us so we can phillet it for you!

