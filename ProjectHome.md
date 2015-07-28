Introduction.

DNS-Discovery is a multithreaded subdomain bruteforcer meant to be
used by pentesters during the initial stages of testing.
It uses a wordlist that concatenates with a given domain to search for
subdomains.

DNS-Discovery resolve and display IPv4 and IPv6.  It's similar to others
tools, like dnsmap, but multithreaded.
It was tested in GNU/Linux 2.6.38 and FreeBSD 8.1-STABLE.

Download

http://dns-discovery.googlecode.com


Compiling
```
$ make
```

Usage
```
usage: ./dns-discovery <domain> [options]
options:
	-w <wordlist file> (default : wordlist.wl)
	-t <threads> (default : 1)
	-r <report file>
	-c <csv report file>

```
ex:
```

$ ./dns-discovery google.com -w wordlist -t 5 -r reportfile
   ___  _  ______    ___  _                              
  / _ \/ |/ / __/___/ _ \(_)__ _______ _  _____ ______ __
 / // /    /\ \/___/ // / (_-</ __/ _ \ |/ / -_) __/ // /
/____/_/|_/___/   /____/_/___/\__/\___/___/\__/_/  \_, / 
                                                  /___/  
        by m0nad

DOMAIN: google.com
THREADS: 5
REPORT: reportfile
WORDLIST: wordlist

accounts.google.com
IPv4 address: 209.85.195.84

ads.google.com
IPv4 address: 72.14.204.112

ipv6.google.com
IPv6 address: 2001:4860:b009::68

...
```

Similar tools

dnsmap
http://dnsmap.googlecode.com/

fierce
http://ha.ckers.org/fierce/

dnsenum
http://dnsenum.googlecode.com/


Feedback

You can send me a email to: m0nad at email.com