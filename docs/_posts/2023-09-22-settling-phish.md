---
layout: post
title:  "Settling Phish"
author: mainphish
tags:
  - content
  - phish
categories: 
  - blog
---

Early this year we commented on the classical phishing email disguised as an
[invoice]({% post_url 2023-02-03-attach-a-phish  %}), which usually contains
a malware-laden attachment. Well, this is a variant of that email:

<pre>
Date: Sep 13, 2023, 10:22
From: Account Payable <previousvictimname@somewhere.com>
To: Clueless Phish <cluelessphish@example.com>
Subject: Settlement release for example September 2023 Ref:543201H
Attachment: Electronic payment confirmation.html 1.8kB

Please do not reply to this email. The contact information for sender is below: Sender's Contact Information Please forward the attached invoices to Accounts Payable for processing. We appreciate your business. 

The information transmitted is intended solely for the individual or entity to which it is addressed and may contain confidential and/or privileged material. Any review, retransmission, dissemination or other use of or taking action in reliance upon this information by persons or entities other than the intended recipient is prohibited. If you have received this email in error, please contact the sender and delete the material from any computer. As a recipient of this email, you are responsible for screening its contents and the contents of any attachments for the presence of viruses. No liability is accepted for any damages caused by any virus transmitted by this email.
</pre>

It comes with an attachment that claims to be a html file. 
We were supposed to inspect the contents but, given the rest of the email, 
we have enough clues to know this is a phishing email.

## Identifying this as a phishing email in easy steps

- The `From:` field contains someone's work email address (which we are 
calling `previousvictimname@somewhere.com` in this email) while pretending to
be from *Account Payable*. 
- The `Subject:` field tries to look serious with some Reference number. 
But, why would it be a settlement? If you do not expect one, chances are you
should not have received it.
- The distaste this phisher has for punctuation should be a dead giveaway.
- Heavy on disclaimers, short on explanation. Once again, that is to make it
seems legalese, which would imply important, and which in turn would hopefully
make someone click on the attachment. 
- *No liability is accepted for any damages caused by any virus transmitted by this email.* Oh, really? Thanks for the warning!
- *As a recipient of this email, you are responsible for screening its contents and the contents of any attachments for the presence of viruses.* Which is what
we are doing here: this email has been screened to be dumped (or added to your
phishing pholder).
- No "*kindly*" this time; that makes me feel sad.

If this email was sent to someone who handles invoices all day, I could see 
said person clicking on the link. 
For the average Joe like you and I, it just screams *phishing* too loud.
Not only my ears hurt but so do my ear wax.
