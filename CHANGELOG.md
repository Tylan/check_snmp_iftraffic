<a name="1.0.1"></a>
# [1.0.1](https://github.com/Tylan/check_snmp_iftraffic/compare/v1.0.0...v1.0.1) (2022-09-23)

### Features

* Added the ability to change SNMP timeout and retry values.

### Other Fixes

* Removed regex option.
* Changed commented section and moved changes to this file.
* Renamed option variables so they can be distinguised as option variables.
* Moved variable defintions around so they are grouped appropriately.
* Changed and improved SIG{ALRM}.

<a name="1.0.0"></a>
# [1.0.0] (Initial Release) (2022-09-22)

* Forked from Greg Frater's check_iftraffic64 version

### Features

* Conversion from Net::SNMP to Net-SNMP
* Added showing all interfaces with --list not just IP based ones.  We sometimes need to monitor L2 ports.
* Added ability to remove certain perfdata.  Removes noise from stuff some might not care about.
* Changed the perfdata output for in_ave and out_ave to keep in line with interface speed and units provided.  Will 
  display 0.80Mbps instead of 800Kbps for example if units are set to m.
* Added an option to be able to disable RX and TX totals on output.

### Bug Fixes

* Fixed perfdata output.

### Performance Improvements

* Created get_results sub to simplify some code.
* Cleaned up some code where appropriate.
* Fixed perfdata to conform to Nagios semicolon standards: https://nagios-plugins.org/doc/guidelines.html
