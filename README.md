# TPLink-Archer
Command-line tool to get TPLink Archer router configuration.

I created this tool to solve an issue with my TPLink Archer MR600 router and now I find it useful to
get various information from it w/o using the  web interface.
Basically, it can be used to get the configuration information available on the main page on the
web interface, e.g.: ISP, Network configuration, DNS information, usage statistics, HW/SW version,...

```usage: archer.py [-h] [-d] [-f [FILE]] [-r HOSTNAME] [-u USERNAME] [-p PASSWORD] [-P PROTOCOL] [-i]

Get TP-Link Archer router current configuration, as shown on the first page after login

optional arguments:
  -h, --help            show this help message and exit
  -d, --debug           print debug messages (to stdout)
  -f [FILE], --file [FILE]
                        write debug messages to FILE (default to <hostname>-debug.txt)
  -r HOSTNAME, --router HOSTNAME
                        TP-Link Archer router IP address/name (default to 100.72.0.41:4433)
  -u USERNAME, --user USERNAME
                        Username to use for login (default to admin)
  -p PASSWORD, --password PASSWORD
                        Password to use for login
  -P PROTOCOL, --protocol PROTOCOL
                        Protocol to use (http/https)
  -i, --info            print version and exit
```
Will generate a config file if none exists.

