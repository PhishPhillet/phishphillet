---
layout: post
title:  "Phone Phish"
author: mainphish
tags:
  - content
  - phish
  - goodphish
  - email
  - zabbix
categories: 
  - blog
---

You all know I like to show appreciation for those who can put together a
good phishing email/text/call/whatever. As this example will show, you do not
need to make it fancy to work; a short clever one will do just fine!
Now, it is in Spanish, but who cares? We've had them in 
[German]({% post_url 2023-12-08-swiss-phish-message %}) 
before, and I need to put up the ones people sent me that were in French and
Russian. But, I am getting ahead of myself: let's admire today's phishing email
(apologies for removing the accents but I have not figured out yet how to
preserve them):

<pre style="white-space: pre-wrap; font-family: monospace;">
From: Zabbix Latam <marketing.latam@zabbix.com>
Reply-To: marketing.latam@zabbix.com
Date: Thu, Aug 21, 2025 at 3:27 ¯PM
Subject: Zabbix Forum Mexico 2025 - Participacion confirmada
To: Clueless Phish <cluelessphish@phishphillet.com>

Ver en el navegador

Hola ,
======

Gracias por registrarte para el Zabbix Forum Mexico 2025! Nos complace
informarte que tu participacion ha sido confirmada. A continuacion,
encontraras los detalles del evento:

- Fecha y hora: 5 de noviembre de 2025
- Ubicacion: Ciudad de Mexico
- [Sitio web oficial del evento]

Esperamos verte alli.  Si tienes cualquier duda, no dudes en escribirnos 
a markeeting.latam@zabbix.com.

Saludos cordiales,
Equipo de Zabbix
</pre>

So the gist of said email is that my registration for the Zabbix Forum 
Mexico 2025 was successful. Now,
[Zabbix](https://www.zabbix.com/) is a well known -- even I have used it -- 
network monitoring system. 

## Why it is well done ##

- Given my line of business 
(cybersecurity and data privacy), it makes sense that I may go to that
event. So, sending an email saying I had registered for it indicates
they did some research.
I would even considering checking the link (which I did but not the way
they expected me to do).

- The email addresses used in the email --  `marketing.latam@zabbix.com` --
has the right domain for Zabbix. None of that junk gmail we usually see. 
They put the effort here. I like it. 

- The link behing `Sitio web oficial del evento` starts with 
`http://go.pardot.com/`.  That is a marketing and sales platform
[owned by Salesforce](https://www.salesforceben.com/what-is-pardot-used-for/), 
which in turn is well known in the marketing and customer service arena.
A lot of companies offering
webinars and conferences love their tracking links and salesforce crap.
The fact these phishers got an account there makes me feel all warm and
fuzzy.

Overall I am glad to have received this phishing email (yes it was directed
to me instead of something someone else sent to me). It restores my faith 
in the phishing community.

## If it was so good, why didn't you click on it? ##

- First of all, the `Hola`. Isn't that a bit too chummy? Why not start with
`Congratulations in Spanish!` or something like it?

- I knew I did not sign up for any Zabbix conference this year, be it in Mexico
or the Moon.

- I hate tracking links. With passion. I will email back the sender, if it
smells legit, or find another way to get a track-free link; just ask 
[NIST](https://www.nist.gov).

- Also, I do not like to click on links or open QR codes just because I 
receive them.
