---
layout: post
title:  "Phisher Can't Paypal"
author: mainphish
tags:
  - content
  - phish
  - lazyphish
  - badphish
  - paypal
  - email
  - gmail
categories: 
  - blog
---

Some people can't dance. Others can't bake, from pasta to a brownie, to 
save their lives. I
fit neatly in that second group. And then there are those who 
can't write a beliveable PayPal phishing email. Guess which group our 
phisher belongs to?  Exactly. 

We have seen some bad phishing emails before. Some of which are bad enough
they are interesting or entertaining. Today's example is none of that. 
Without further ado, let's jump right into it:

<pre style="white-space: pre-wrap; font-family: monospace;">
From: avenbuankate242@gmail.com
Date: Thu, 31 Jul 2025 10:50:10 -0700 (PDT)
X-Google-Original-From: PayPal,Inc.
Subject: Invoice for order no KMWTQ9X714 82365544640 3018-VC-2491
To: Clueless Phish <cluelessphish@phishphillet.com>


PayPal,Inc.
Date: 2025-07-31
Invoice No: 60923-9889

Your order receipt.

Dear Clueless Phish,

We've noticed an unusual charge on your PayPal,Inc. account. If it's 
unauthorized, call to cancel. Otherwise, 377.35 USD will be billed today.

Your Product is processed. If you have any inquiries, please reach out to us.
Product: Sephora Gift Card
Tracking No: 2410995-10733
Quantity: 1x
Amount: -377.35 USD
Issues with this Invoice?
Call +18482515821 to report any unauthorized Invoice.

PayPal,Inc. is committed to preventing fraudulent emails. Please do not 
reply to this email. To get in touch, call the toll free number provided in 
the email.

Thanks & Regards,
PayPal,Inc.
</pre>

## How can I name all that is wrong in this phishing email?

- Phisher could not be less bothered with creating a believeable email address.
Yes, he used gmail since, just like with Microsoft's outlook, creating an email
is easy peasy. Could he make it sound paypal-ish? Oh no, that would be too 
much to ask! Instead we have `avenbuankate242@gmail.com` which is, well, 
come on!

- Phisher was not satisfied with having a non-believeable email: he could 
not be bothered to hide it, say writing it as 
`PayPal Support <avenbuankate242@gmail.com>`. So, now we have this email
address screaming "look at me! I am suspicious and have nothing to do with
the company I am impersonating!" Is that too much to ask?

- How many invoice numbers do you need to mention in the `Subject:`? Do you
think that by coming up with more people will take it more seriously? Or do
you are trying different invoice number formats in hope one looks like what
the potential clueless phish has seen before, and as a result looks more
legit?

- This email is plain text. While I like plaintext emails from the security
standpoint, *this is a phishing email!* It is supposed to be insecure. I do 
not mean insecure enough to trigger a phishing/spam filter, but it could use
a bit more vibrance! A typical paypal email is html-based, with its evil
tracking pixels and other privacy stealing features. Also, it has the paypal
logo on it. Can't you copy the logo and attach it inline? Or get the look believeable? What is wrong with you?

- Talking about the look, the flow of the email, as in of which words are being
used and how they are laid in the email are better described as the result of 
someone trying to put together a paypal phishing email during lunch based on 
what he heard during a phone call a few hours earlier, when he did not have
a way to take notes. In other words, it is the phishing email equivalent of
the Pontiac Aztek. Hint: there are programs out there who will take care of
your phishing emails from creating something, ahem, *believeable* to tracking
the response and getting the malicious links or payload just right. There
is no shame if you cannot write a phishing email on your own, but like the
old TV ad said, get some help!

<img src="/images/2025/stop-it-help.jpg"
class="align-center" alt="[Man in suit ssaying stop it, get some help]">

As I admitted earlier in this post, 
I have no baking skills, but I feel while my attempts at making 
brownies set a really low bar. Ok, not as low as the extremely
[lazy phisher]({% post_url 2023-11-17-humanitarian-phish %}) we talked about
a while ago, but pretty bad regardless. I was wrong.
This phisher looked at my accomplishment, said
"hold my beer!", and showed a new low bar could indeed be set, that the 
race to the bottom is far from over.

Did he get there by accident, concidence, just lack of skills, or did he woke 
up in the morning and decided to a really disappointing phishing email?

You decide.

## That is rash! Are there any redeeming features?

- Well, if I had to pick something, the best I can do is the statement
"do not reply to this email." Most such real emails like to have a
`noreply@domain.com` kinda of email address, implying if you reply to it,
it will be ignored. So that specific bit of the phishing email is
appropriate. But, I had to squint really hard to find it!
