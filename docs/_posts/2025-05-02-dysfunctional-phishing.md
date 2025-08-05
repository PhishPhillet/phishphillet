---
layout: post
title:  "Dysfunctional Phishing"
author: mainphish
tags:
  - content
  - phish
  - era
  - eft
  - claim
  - secure
  - insurance
categories: 
  - blog
---

We have covered some great phishing emails,
some terrible ones, and some that are so bad they are good. 
Today's example fits neatly in the latter category. First we need to 
admire it in its glory:

<pre style="white-space: pre-wrap; font-family: monospace;">
From: "Aetna"<invoice+statements+acct_1m9sewj6dkcrlux4@auth.com>
Date: 30 Apr 2025 00:36:36 +0200
Subject: AETNA ERA/EFT Claims -  Attention Required
To: Clueless Phish <cluelessphish@phishphillet.com>

[Logo]

"ERA/EFT" AETNA
sent you a secure message

                 [view secure message]

The first time you access it you'll be asked to enter your email address

You can view your message at any time afterwards in our [Secure Messaging Portal].
	
 
2020 Mimecast Services Limited and affiliates. The information contained in this communication is confidential and may be legally privileged. It is intended solely for use by the intended recipient. If you are not the intended recipient, or authorized to receive it, any disclosure, copying, distribution or reliance of the contents of this information is strictly prohibited. For information about how your personal data is processed through this service, read the Mimecast Secure Messaging Privacy Statement.
</pre>

<img src="/images/2025/Dysfunctional.jpg"
class="align-center" alt="[Meme where Buzz Lightyear from Toy Story says 
'dysfunctional everywhere' while Woody looks terrified]">

## Why is it a classic
I know, I know, it is not long, nor has fancy images besides the logo (I may
upload it later after checking it for funny business), but there is gold to be
found here; the meme just above this paragraph, and the title of this blog 
entry,
should be a hint.

- These phishers did some right things. For instance, while the email is
suspicious (domain is `auth.com` instead of some AETNA-related one), that
is not unherad of.
I know of a bank when you go to their website and click on login, you are 
immediately sent to a third party site to do the actual login instead of 
having the address suggest we are still looking at a website remotely related
to them. I did contact said bank and they said it is legit.

- The `invoice+statements+acct_1m9sewj6dkcrlux4` could be legit even though
it does not make me happy. It indicates this is an email that is being tracked:
if you reply to it, your reply not only will indicate you replied to this 
specific email but also allows them to associate it with this campaign.
Many *customer relationship managers* allow you the user to do that.
I do not like that from a privacy standpoint but that is a discussion for
another blog.

- The `view secure message` is a shortlink (some of you know how much I despise
them) to the website they created to collect your personal information and
login info. Standard practice on a well thought phishing email.

- Now we get to what makes this a classic: [AETNA](https://www.aetna.com/) is an American [managed health care](https://en.wikipedia.org/wiki/Managed_care) company (think [Insuricare](https://the-incredibles.fandom.com/wiki/Insuricare) from the movie The Incredibles).

- However [Mimecast Services Limited and affiliates](https://www.mimecast.com/company/) 
is a company that manages -- think security, archiving -- business emails 
hosted in Google (Gmail) and Microsoft (O365, Exchange, Outlook).
AETNA is not a business made by two people in a garage; they can afford
to make sure all their communications reflect their corporate image.
If this is a phishing email pretending to be an email from AETNA, why would
half of the email be mentioning Mimecast? Even if the real AETNA used Mimecast,
that would be done behind the curtain. This phishing email should represent
AETNA and AETNA alone.

- So this phishing email looks like two distinct ones that were combined for
some mysterious reason. Was the phisher in a hurry and got overly excited
with cutting-n-pasting? Was he trying to merge two phishing emails thinking
if a potential victim ignores the first part of the email, said victim would
fall for the second part? Was it done as a bet?

- Last but definitvely not least, the other think, `Secure Messaging Portal`, 
goes to an url in `mimecast.com`. No, I will not post it here just in case
Mimecast never bothers to disable it.
Howerver, if that was also set up by the phisher, that would tell a lot about 
Mimecast.

Why I do like this phishing email? It is dysfunctional: it combines best
phishing email composing practices, clever ideas, with rather confused
execution. It has something for everyone. Perhaps different groups were 
assigned different tasks in creating this phishing email, and then they
all sent their work to someone who just slapped it all together and sent it.

