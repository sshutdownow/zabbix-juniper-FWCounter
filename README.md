ZBX-JUNIPER-FWCounter
==============

This template uses the SNMP to discover via LLD FWCounters on JunOS devices, that are support JUNIPER-FIREWALL-MIB.


Items
-----

  * Discovery: jnxFWCounterFilterName
  * Discovery: jnxFWCounterDisplayType
  * Discovery: jnxFWCounterByteCount
  * Discovery: jnxFWCounterPacketCount

Triggers
--------
  * None

Graphs
------

  * Discovery: jnxFWCounterByteCount

Installation
------------

1. Add a value mapping named `jnxFWCounterDisplayType` with the following values:
  * 1 ⇒ other
  * 2 ⇒ counter
  * 3 ⇒ policer 
2. Import **zbx-junos-fwcounter-template.xml** file into Zabbix.
3. Add to your host the **{$SNMP_COMMUNITY}** macro with your SNMP community as value.
4. Associate **ZBX-JUNIPER-FWCounter** template to the host.

### Requirements

This template was tested for Zabbix 2.2.0 and higher.There are no additional requirements.

### Copyright

  Copyright (c) 2016 Igor Popov

License
-------
   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

### Authors

  Igor Popov
  (ipopovi |at| gmail |dot| com)
