# TryHackMe DNS in detail write-up
DNS also known as domain name system translate IP addresses like 136.164.32.2 to something that is easier to read and remember, a web URL like Tryhackme.com or linux.org.

## Task 1 
* What does DNS stand for? **Domain Name System**

## Task 2
There is a heirarchy to these web URL that the DNS server providers translation for this is a simple graph  showing a basic idea of how this heirarchy works (This does not show up well on dark mode I'll fix that at some point)
![domain_levels](https://user-images.githubusercontent.com/64501695/160914980-7500582b-d318-4eec-872f-5e8a95be807d.png)

* What is the maximum length of a subdomain? **63**
* Which of the following characters cannot be used in a subdomain ( 3 b _ - )? **_**
* What is the maximum length of a domain name? **253**
* What type of TLD is .co.uk? **ccTLD**

## Task 3
There are many different record types for DNS, many of these record types are just for the DNS to reference but others can also be viewed and understood by people

**A record** Resolves IPv4 addresses
**AAAA record** Resolves IPv6 addresses
**CNAME record** Is used to give your domain name an alias or another name to reference it by
**MX record** Is a record used for handling mail
**TXT Record** Are the records that can be read by humans where any type of useful information can be stored

* What type of record would be used to advise where to send email? **MX**
* What type of record handles IPv6 addresses? **AAAA**
