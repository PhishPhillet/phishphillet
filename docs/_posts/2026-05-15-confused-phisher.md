---
layout: post
title:  "Confused Phisher"
author: mainphish
tags:
  - content
  - phish
  - badphish
  - funphish
  - email
  - subscription
  - service
categories: 
  - blog
---

Those of you who have been reading this site know how I love phishing messages
that are so bad they are good. 
[Last week's post]({% post_url 2026-05-01-phish-has-a-bimmer %}) was not one
of them. In fact, it annoyed me to no end.
I am glad to say a phisher rose (or lowered; you decide) to the occasion and
gifted me with a disaster.

At first glance, this phishing email seemed to be similar to the last one 
in type: some kind of subscription phishing email. 
It is... but it is not at the same time. 
I do not think it knows what it wants to be, nor what punctuation looks like.
Withotu further ado, gaze upon its majesty:

<pre style="white-space: pre-wrap; font-family: monospace;">
Date: Friday, May 15th, 2026 at 6:58 PM
From: Supabase <welcome@supabase.com>
Subject: ra.xgit.an@gmail.com has invited you to join Your protection 
service renewal will auto-charge 365 USD Please call +1 (805) 727-9586 
for assistance Reminder: Norton Subscription Payment
To: Clueless Phish <cluelessphish@phishphillet.com>

You have been invited to join Your protection service renewal will 
auto-charge 365 USD Please call +1 (805) 727-9586 for assistance 
Reminder: Norton Subscription Payment.
==========================================================================================================================================================================

Your protection service renewal will auto-charge 365 USD Please call 
+1 (805) 727-9586 for assistance Reminder: Norton Subscription Payment is 
an organization owned by ra.xgit.an@gmail.com.

[Join this organization]


What happens when I join an organization?

You will have access to all the projects of that organization. If you do 
not recognize this organization, please contact our team at 
support@supabase.io


</pre>

`[Join this organization]` is the link to the phishing site... or so I hope.
Remember everything here is weird.

## Why I like this  phishing email

Let's ignore the obvious telltale sign of using 3 completely different
email -- `welcome@supabase.com`, `support@supabase.io`, and 
`ra.xgit.an@gmail.com` -- addresses.
This is the phishing equivalent of a train crash unfolding slowly:

- The `Subject:`! Oh, the `Subject:`! It looks like the body of an email
was rear ended by the subject of another email (or the same one; we are
talking about disaster here). But wait, there is more! It is gigantic:
try reading it aloud in one breath.

- I mentioned before the lack of punctuation, but in all honesty I doubt
it would have saved it; the sentence beginning with
`You have been invited to join Your protection service renewal` is really at
least two sentences associated with two distinct emails crashed together.
Maybe my train analogy is correct, but this train did not derail.
It actually crashed into another train and cars flew all over the place.
Maybe a truck also joined the fun.

- There is a long series of `====` that are just thrown there for
good measure. The message body multiple train crash continues after that.

- It asks `What happens when I join an organization?` I don't know, man!
Maybe a singularity will be formed?
I am trying to back away from it so I can try to get the gist of it, but 
right now I am still confused. 

- `Norton Subscription Payment is an organization owned by ra.xgit.an@gmail.com.`
Maybe this transcends language as we understand it. This is post post modernism?
I do not know if I should ask a grammar teacher, an art expert, 
a phylosopher, or a witch 
doctor to explain this. Or maybe get all of them in the same room.
What would Schroedinger say?


## We need your help!

I try to post samples of good, bad, and weird phishing messages here but I 
can only do so much on my own. I need your help! If you receive a 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">phishing message</a> </b>
-- email, text, or even voicemail, and want me to tear it apart and
make fun of it, send 
<b><a href="mailto:{{ site.email | encode_email }}" title="Feed the Phish">the phishing message</a> </b>
to us so we can phillet it for you!

