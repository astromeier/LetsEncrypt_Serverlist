# LetsEncrypt_Serverlist
LetsEncrypt does NOT recommend to use a list of their verification servers as they can change without notice!

In some cases it could be useful to whitelist the servers used by LE.
This list is updated from time to time.
It is very probable that LE will change some of their servers and this is not reflected in this list asap....
This Serverlist contains IP addresses whose server names do not indicate Lets Encrypt.

In addition you'll find the FQDN-List. These server names are often used to start a verification process and should also be whitelisted.

Motivation:
My firewall is quite nailed up with geo-ip-lists and e.g. the free AbuseIPDB-List - and when a LE server is blocked the certificate validation fails!
I've seen some entries of LE IP addresses in lists like AbuseIPDB - but I'm sure that the whitelisting is ok:
The logged acme challenges and querys come from different IP addresses and when the same challenge comes from a known letsencrypt FQDN server, too I assume the whitelisting is ok....
