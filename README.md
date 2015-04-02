# blcheck

A powerfull script for testing a domain or an IP against mailing black lists.

Features
--------------------

* More then __200 black lists__ already included!
* Automatic distinction between __domain or IP__
* Performs __PTR validation__ (only if domain is supplied, does not work for IP)
* The result of script is the number of servers which blacklisted the domain, so it can be used for any kind of __autonomated scripts like cronjobs__
* 3 verbose (-v) levels and a quite (-q) mode
* Informative and pleasant output

Requirements
--------------------

* Any linux distribution wih bash


Usage
--------------------

#### With root access
1. Download the script to your /usr/bin folder
2. Type `chmod +x /usr/bin/blcheck`
3. Type `blcheck <domain_or_ip>`
4. Wait for the answer, it might take some time


#### Without root access
1. Download the script to your system
2. Type `chmod +x /path/to/blcheck`
3. Type `/path/to/blcheck <domain_or_ip>`
4. Wait for the answer, it might take some time


Inapp help
--------------------
	Usage: blcheck [options] <domain_or_IP>

	Supplied domain must be full quialifined domain name.
	If the IP is supplied insead the PTR check cannot be executed and will be
	skipped.

	-v    Verbose mode, can be used multiple times (up to -vvv)
	-q    Quiet mode with absolutely no output
	-h    The help you are just reading


Credits
--------------------
Script has been written by the [Intellex](http://intellex.rs/en) team.
