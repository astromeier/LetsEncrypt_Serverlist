# LetsEncrypt_Serverlist
LetsEncrypt does NOT recommend to use a list of their verification servers as they can change without notice!

Starting 2025 I use a ASN List Alias for temporary whitelisting when the ACME verification process is ongoing.
Please use file LestEncrypt_ASN.txt

===
OLD and obsolete:
===

**As LE forces its cloud verfication (https://letsencrypt.org/2020/02/19/multi-perspective-validation.html) it becomes more and more senseless to use a list of single IPs. Actually LE uses AWS Servers, but plans to use more cloud providers.
I try to identify IP ranges or ASN numbers for future - but don't think that works.**

**My workaround: I disable the firewall rules manually for a moment and renew my certificates in that period...**

In some cases it could be useful to whitelist the servers used by LE.
This list is updated from time to time.
It is very probable that LE will change some of their servers and this is not reflected in this list asap....
This Serverlist contains IP addresses whose server names do not indicate Lets Encrypt.

In addition you'll find the FQDN-List. These server names are often used to start a verification process and should also be whitelisted.

Motivation:
My firewall is quite nailed up with geo-ip-lists and e.g. the free AbuseIPDB-List - and when a LE server is blocked the certificate validation fails!
I've seen some entries of LE IP addresses in lists like AbuseIPDB - but I'm sure that the whitelisting is ok:
The logged acme challenges and querys come from different IP addresses and when the same challenge comes from a known letsencrypt FQDN server, too I assume the whitelisting is ok....

**In discussions some users brought up IP addreses I've never seen at my location in Germany. I assume that there are additional verification servers in other regions of the world. So please let me know your findings...**

A valuable source I recently found (2020): https://robotsdb.de/lets-encrypt-validation-server/
