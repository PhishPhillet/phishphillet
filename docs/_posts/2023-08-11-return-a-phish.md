---
layout: post
title:  "Return a Phish"
author: mainphish
tags:
  - content
  - phish
categories: 
  - blog
---
In the end of last month I received this uninspiring but not badly
put together phishing email. 
I will start with saying this email is completely not in the same league
as the phishing one we covered in the previous post.

<pre>
From: example.com <info@a.daucu.com>
Date: 31 Jul 2023 08:34:28 -0700
Subject: Returned Mail.
To: Clueless Phish <cluelessphish@example.com>

**Returned Mail.**

Attention:

Some emails sent to your account cluelessphish@example.com are being 
bounced back due to sync errors.

Kindly follow the instructions below  to resolve this problem.
INSTRUCTIONS [*link to phishing site goes here*]

If you have already solved this problem, kindly ignore this message.
example.com Online Team.

This message was sent by the system for notification purposes only. 
Please do not reply.
</pre>

## Identifying this as a phishing email in easy steps

- Our old friend, *kindly* is back. Twice, as if that added more weight.
- This phisher is pretending to be from the "*Online Team*" (whatever that
means) of the company the intended target -- the mark, 
a.k.a.  *Clueless Phish* -- works at. 
To protect the innocent, the domain was renamed to `example.com`. 
Thing is that is done rather badly: unless we are reading this in Microsoft 
Office, you can see the email address in the `From:` field has nothing to do 
with the mark's.
- The idea here is for the email recipient to panic because of the bounced 
emails, and click on the malicious link. This specific part of this email 
is almost good enough: most people will not hover their mouse over the link to 
find out where it goes.
- The last line was clever enough to say, in its own way, that the email
address used to send the email is not monitored, so do not reply to it.
But the wording could have used some help. Still, they were trying to do a 
proper phishing email.

Would this phishing campaign work? Possibly if the victim does not slow down to read.
It is trying to be a proper phishing email, but it does not have the
magic last one had.
I really cannot say anything really good or bad about this phishing email
besides, well, there it is.
