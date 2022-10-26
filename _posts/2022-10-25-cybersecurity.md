---
title: "DoS attacks!"
date: 2022-10-26T00:00:00+03:00
categories:
  - blog
tags:
  - cybersecurity
  - ddos
---

At this article you will find explanation of few cyber security attack methods, a tool that can be used for the attack and how to prevent it. 
It will be a minimal guide for the user to understand those attacks and use them as well.  

# DoS (Denial of service) attack

## Definition:

Based on [CISA.gov](https://www.cisa.gov/uscert/ncas/tips/ST04-015) (Cybersecurity and Infrastructure security agency): the DoS attacks happen when the attacker flood a network of requests to stop the services, the attacks may include servers, email, banks or websites.

## Types: 

Here are the types of the DoS attacks: 

* DDos 
* DRDoS 

[source](https://www.clouvider.com/blog/dos-ddos-and-drdos-what-is-the-difference/)

## Tools: 

there are couple of tools that can be used for this attack, having a comparison between them would be awesome, yet here are some of them: 

- GoldenEye
- Slowloris
- LOIC (Low Orbit Ion Cannon)
- HOIC (High Orbit Ion Cannon)
- THC-SSL-DoS
- HULK (http Unbearable Load King)
- Pyloris
- TOR's Hammer
- XOIC
- RUDY (R U Dead Yet ?)
- DAVOSET
- OWASP HTTP POST

[Resource](https://www.javatpoint.com/best-ddos-tools-for-kali-linux)

The blackarch linux has more than 30 tools of DoS attacks tools that are listed on their website: [Resource](https://blackarch.org/dos.html)
You can check the kali linus tools as well from this [website](https://www.kali.org/tools/)

### Demo: 

Today we are going to show a simple demo for slowloris tool with Jekyll local server, 


[This link](https://jekyllrb.com/docs/) explains how to start a local jekyll server.


As for the tool we are going to use a simple attack with python here is 

```
python3 slowloris.py websiteOrIP -p PORT -s 500 
```

The port is not mandatory. 

## Prevention: 

Based on [cloudflare](https://www.cloudflare.com/learning/ddos/ddos-attack-tools/how-to-ddos/) a well-known and well used server provider, there are couple to tactics that can be used to prevent the DoS attacks:

which are: 

- Rate limiting 
- Firewalls
- Anycast 

Further reading: 

- [Great article with full details](https://www.comparitech.com/net-admin/dos-vs-ddos-attacks-differences-prevention/)
- [Anycast network](https://www.cloudflare.com/learning/cdn/glossary/anycast-network/)