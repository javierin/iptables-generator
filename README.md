## Iptables generator for a honeypot fail2ban filter

**You can _immediately lock yourself out_ if you don't have appropriate fail2ban ignoreip rules**

This python script reads a text file with ports (one per line) and outputs the required
multiport iptable rules needed to generate a honeypot in fail2ban.
I have included the most commonly scanned ports for services I mostly don't use.
Should you need to add extra honeypot ports, just add them each in one line.

**AGAIN** Please be aware that I include port 22 as a default.

Installation
------------
Just clone the repo and check if ports.txt fits your needs.

I personally prefer to add the output of the command to a script run at boot time.

The rest of the fail2ban honeypot is explained in this spanish language blog post, should be easy to translate using your favorite online translator.

