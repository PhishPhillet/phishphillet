---
layout: post
title:  "Short Phish"
author: mainphish
tags:
  - content
  - phish
  - shortlink
  - bank
categories: 
  - blog
---

Those who know me are aware of my low opinion about tracking links in general
and URL shorteners specifically. 

By default, I despise them because they are used to violate the privacy of 
the email recipient by collecting personal (using the GDPR definition here)
information from any recipient who clicks on the link. Companies using them
argue there is a legitimate interest to collect that data, namely 
to verify the effectiveness of their marketing campaign. Well, GDPR 
will say that marketing is never a legitimate reason to collect personal data.

Now, knowing whether your phishing email was effective is something the more
sophisticated phisher would be interested on. After all, the best commercial
rent-a-phish tools do produce reports telling how many emails were opened 
and, of those, how many had their links clicked.

But wait! There is more! Tracking links also make it that easier for phishers 
to hide their intention: they do not need to go to a "phishers-only" service:
any commercial tracking link/
[URL shortene](https://zapier.com/blog/best-url-shorteners/) 
service will gladly take their money.
Case in point is the next phishing email:


<pre>
From: "Bank of America" <accounting@mysecureprotection.com>
To: Clueless Phish <cluelessphish@example.com>
Subject: You Have A New Message
Date: 14 Nov 2024 02:40:56 +0100


Activity Alert
You Have a New Message

Dear Customer,

We're letting you know that you have a new message in your Online Banking mailbox.

Please [**Login Here to view the Message Center**] and read your message.

We encourage you to read the entire message, because it contains specific information about your account.

If you haven't done so already, you can go paperless now. It's a safe and secure way to help stay organized. 

We're here to help. If you have questions, contact us online or call the number on the back of your credit or debit card.

We'll never ask for your personal information such as SSN or ATM PIN. If you get an email that looks suspicious or you are not the intended recipient of this email, don't click on any links. Instead, forward to abuse@bankofamerica.com then delete it.

Please don't reply to this automatically generated service email.

Privacy Notice     Equal Housing Lender  

Bank of America, N.A. Member FDIC
© 2024 Bank of America Corporation
</pre>

## But, this looks like a typical example of the classic phish with a link

Right you are, and we can see other telltale signs of a phish at large:

- Interesting grammar
- If you do not have a *Bank of America* account, receiving such email is a dead giveaway.
- I was going to make fun of the subject of this email, 
"*You Have A New Message*", but banks and credit card companies are notorious
for having suspicious Subjects. While they claim that is done to "make it 
harder for malicious attackers to immitate them," the reality is as if they 
are trying to copy thge phishers. While I appreciate them having something to
strive for, that is not what they should be aiming for.
- Same goes for the return email address. I am sorry but it sure looks 
suspicious: why would *Bank of America* not use `bankofamerica.com` for its
return address? I would love to say "Aha! That is another dead giveaway!"
but I could name 3 other banks who have cutesy addresses for who knowa why.
Still, it is suspicious in my book, so I would not click on the link.

But this phish has a twist. Behind the 
"[**Login Here to view the Message Center**]" is a short link. Specifically, 
a `t.co` links which indicate it was created using 
[Twitter/X's link service](https://help.x.com/en/using-x/url-shortener).
I expand the link, and it goes to `https://cameoutair.com/bl2/jsde5/SOME-PAGE.htl` (I do not want you to accidentally click on their site). 
Do you remember when I talked about suspicious sites ealier on?
I do not think (or **hope**) that `cameoutair.com` is a domain owned by
Bank of America. But, the only way to figure out that the link was even
more suspicious was to expand the shortened link.

Bottom line is phishers are getting better as they are making use of 
sleazy commercial products like link shorteners.

## What should I do then?

1. Just say no to link shorteners and tracking links!
1. If you receive such email and do have a Bank of America (or whatever bank
you use) account, **do not click on the link!** Login into the official bank's
website and see if there is a message. If not, contact their support.
Yes, I know that can be frustrating but it is the only way to be sure.
