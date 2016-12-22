[Device42](http://www.device42.com/) is a comprehensive data center inventory management and IP Address management software
that integrates centralized password management, impact charts and applications mappings with IT asset management.

This repository contains sample script that link ServiceNow and Device42 back and forth.

## Assumptions
-----------------------------
    * This script works with Device42 10.5.0.1473709546 and above

### Requirements
-----------------------------
    * python 2.7.x
    * requests (you can install it with pip install requests or apt-get install python-requests)

### Usage
-----------------------------
	* For proper run script you need to add mapping.xml, then put credentials and fields as in sample
	* (!IMPORTANT) For each ServiceNow table that in mapping.xml you should add 'u_device42_id' custom field
	* For proper run script you need to edit mapping.xml, put fields as in sample

Run the script and enjoy! (`python sync.py`)
If you have any questions - feel free to reach out to us at support at device42.com


### Compatibility
-----------------------------
    * Script runs on Linux and Windows


### Info
-----------------------------
    * mapping.xml - file from where we get fields relations between D42 and ServiceNow
    * lib.py - file with integration description, we describe how fields should be migrated
    * sync.py - initialization and processing file, where we prepare API calls


### Support
-----------------------------
    This ServiceNow mapping / sync script is provided as-is without any support. We do provide fee-based professional services/support if you need help with this script.  To find out more please email sales@device42.com with subject ServiceNow script support.


