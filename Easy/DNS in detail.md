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

## Task 4
In order to get a response from a DNS server with the information you requested many different types of servers need to queried. This graph shows a basic overview of what that looks like 
![dns](https://user-images.githubusercontent.com/64501695/160916325-3c2a6589-f811-498d-b27a-7d9b457e07db.png)
* What field specifies how long a DNS record should be cached for? **TTL**
* What type of DNS Server is usually provided by your ISP? **recursive**
* What type of server holds all the records for a domain? **authoritative**

## Task 5
This is the pratical part of the room and it requires to view the provided site in order to get the answers
* What is the CNAME of shop.website.thm? **shops.myshopify.com**
* What is the value of the TXT record of website.thm? **THM{7012BBA60997F35A9516C2E16D2944FF}**
* What is the numerical priority value for the MX record? **30**
* What is the IP address for the A record of www.website.thm? **10.10.10.10**
