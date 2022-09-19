# check_iftraffic64
Nagios and Icinga Plugin for Checking Interface Traffic

### Prerequisites

Perl >= 5.10

Net-SNMP: http://www.net-snmp.org/

Want AES-192 and AES-256 support?  Compile as such:

```
./configure --enable-blumenthal-aes [--bindir=/usr/bin]
make
make install
```

Usage of bindir is optional.  Use at your own risk!
