---
layout: post
title:  "Messaging Swiss Phish"
author: mainphish
tags:
  - content
  - phish
  - image
categories: 
  - blog
---

Most of the phishing we have talked about comes by email, but that does not 
have to be the only way. A more sophisticated phisher knows there are other
alternatives, such as the
[voice mail]({% post_url 2023-10-20-talkie-phish  %})
we previously commented on, and chooses the right attack vector for the right
target. Today we will once again step away from emails and talk about one 
I consider particularly effective: *messaging*.

The main issue I have with messages is that they make it much easier to hide
the sender's true identity
and the true colors of any attachment or link: I usually have to 
cut the url and paste it to a text-only editor to see what the link
actually is. Sometimes even that is not possible: once I was in a Zoom call
where a link supposedly from the host was posted in the chat. I could not
copy it; the only option I had was to open it, which I did not.

The second issue is if this was an
email, people may be more trained to ignore it for a bit or contact their
IT/Security team (or mom) to see if it is fake. But, if this message pops in 
their phone, just that may cause them to click on the link.
Remember there may not be an easy way to copy the message so it can be 
checked; screen capture may be the best you can do here.

Todays example is a message pretending to come from the Swiss Post. 
And, yes, it is in German.

<img src="/images/2023/phish21.png" 
class="align-center" alt="[Phishing message pretending to be from the 
Swiss Post Office]">

Here is the text version.

<pre>
vtweour506748@icloud.com
Heute, 10:58

Schweizerische Post: Ihr Paket is im Lager angekommen, wurde jedoch aufgrung
unklarer Addressinformationen zurueckgehalten und ist nichtzusterllbar.
Bitte
besaetingen Sie innerhalb von Studen Ihre Addresse in Link.

https://correos1.biz/x1

(Bitte antworket Sie mit "Y" beeden Sie dann SMS und oeffnen Sie den
SMS-Aktivieerungslink oder kopieren Sie den Link und oeffnen
Sie ihn in Safari.)

Einen schoenen
Tagwuenscht Ihnen das Team der Schweizerische Post.
</pre>

Here is a (lousy) translation to English:
<pre>Today, 10:58

Swiss Post: Your package arrived at the warehouse, but was held back due 
to unclear address information and cannot be delivered. Please enter your 
address in the link within hours.

https://correos1.biz/x1

(Please answer with "Y" then exit SMS and open the SMS activation link or 
copy the link and open it in Safari.)

The Swiss Post team wishes you a nice day.</pre>


## Identifying this as a phishing email in easy steps

The phiser had a great idea to use messaging to send the attack, but his 
implementation had a lot to be desired.

- The message follows the classic "we have an order that you may or not have
done but need to click on this malicious url or attachment to verify." 
It even tried to add some tension by giving a short deadline. 
- Before you ask, *we* do deal a lot with GDPR and the Swiss Privacy Laws and 
receive correspondence from Europe.
Therefore, *in our case* receiving messages from the Swiss Post may make sense.
However,
- Why would the Swiss Post send a message? I know some people let vendors
and the post office/USPS/FedEx send text messages. But, **we** do not like
to do that.
- We mentioned early about how easy is to hide the sender's identity in a
messaging system. Well, this phisher was napping whan that bit of information
was being handled out: call me weird, but I do not think that the Swiss Post
would use `vtweour506748@icloud.com` as its official email address.
- The same apply to the link to the phishing site. `https://correos1.biz/x1`
does not feel very Swiss Post-like. 
- `The Swiss Post team wishes you a nice day` is an odd way to end a message.
But that may just be me.

Overall, if this was an email most people would probably see this phishing
attempt for what it is. However, given that it was a message in a small phone
screen, there is something there that may cause more people to click on it.
