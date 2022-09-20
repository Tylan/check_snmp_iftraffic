# check_iftraffic64
Nagios and Icinga Plugin for Checking Interface Traffic

Forked and modified.  Some things could have broke from version I forked from after I converted and modified to meet my specific wants and needs.

### Prerequisites

Perl >= 5.10 for basic functionality.
Perl >= 5.80 for AES-192 and AES-256 support.

Net-SNMP: http://www.net-snmp.org/

Want AES-192 and AES-256 support?  Compile net-snmp as such:

```
./configure --enable-blumenthal-aes [--bindir=/usr/bin]
make
make install
```

Usage of bindir is optional.  Use at your own risk!
