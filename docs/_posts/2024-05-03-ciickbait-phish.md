---
layout: post
title:  "Clickbait Phish"
author: mainphish
tags:
  - content
  - phish
  - mail-merge
categories: 
  - blog
---

The title of this post may be a bit of a misonhonor as any good phishing email
needs to have a good clickbait title so the Clueless Phish will look into it.
This one was a bit more interesting because of the amount of similarly sounding
emails it created and the frequency. Also, its style follows that used by 
marketing firms. 
Here is the list at the time this post was written:

<img src="/images/2024/phish22a.png" 
class="align-center" alt="[List of phishing emails claiming to have news
about  the Bank of Canada suing someone]">

Note the Subjects of these emails all follow the pattern
"*Bank of Canada sues SOMEONE for what he said on live TV*." Here is how one
of them looks like in text:


<pre>
From: info@goldclass.net.au <info@goldclass.net.au>
Date: On Friday, April 19th, 2024 at 11:03 AM
Subject: Bank of Canada sues Tucker Carlson for what he said on live TV
To: Clueless Phish <cluelessphish@example.com>


Tucker talked about an incredible development that has the potential 
to astonish everyone. And everyone was already very interested as soon as 
he began to explain the essence; a call came to the studio from a major 
bank in Spain instructing to immediately halt the interview! What did 
Tucker Carlson say that so outraged the government and banks that they 
now threaten him with legal action? In this article, we have gathered all 
the most important information for you, as the interview is no longer 
available, and there are no guarantees that this article will remain 
accessible for long.

[Find out more]
</pre>

And its quasi-HTML (more on that later) version.

<img src="/images/2024/phish22b.png" 
class="align-center" alt="[the same clickbait email as above but seen in a not
very html-friendly email client]">

## Identifying this phishing email
- I have heard of *Tucker Carlson*. I do not remember (and no, I am not going
to bother to search online) whether he is a politician or works on television, 
but the name sounds familiar. But this *Michael Cera* I have never heard of him
before. Animal, vegetal, or mineral? So, why should I care about what Mr. Cera
said on TV? What about Mr. Carlson, or even some more well-known celebrity?
- Clearly the `Subject:` of this phishing email was targeted at people whose
life is run by what they see on TikTok or email. I, on the other hand, make a
point not to read any email with follows the "*Look! We have some shocking 
news or message you must drop what you are doing and click on it!*" for many
reasons, be it news or some new (junk) product.
- On the same lines of the previous bullet point, the entire text of the email
says nothing useful; it is there, exclamantion points included, for the sole 
purpose of enticing you to click on the `[Find out more]` button. 
- The "*there are no guarantees that this article will remain accessible for long*"
is the sense of urgency that is a trademark of phishing and certain
(tele)marketing emails.
- Do you remember the Subect of the email? It followed the 
"*Bank of Canada sues SOMEONE for what he said on live TV*" format where 
"*SOMEONE*" changed (a bit). Why would the same "news" be posted again but
applied to a different SOMEONE? Yeah right...
- Saving the best for the last: did you notice each email had a different
return address even though it was exactly the same thing? This is done to
(hopefully) evade spam filters, but when you put them all together, you can't
help but go "*wait a minute!*".


Do you remember when I said "*quasi-HTML*"? This email was not opened in 
one of the usual privacy-avert mail clients such as gmail or Microsoft 
Office365 (or whatever name it is using this week). Nor it was received in
social media or
[messages](https://phishphillet.com/blog/2023/12/08/swiss-phish-message.html).
This mail client blocks a lot of bits and bobs, only downloading the text of
email. As a resultsaid email looks much more boring albeit more secure and
privacy protecting. In other words, it does not help marketers or phishers.
