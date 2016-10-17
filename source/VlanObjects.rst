Vlan Model Objects
=============================================================

*config/Vlan*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| VlanId **[KEY]**   | int32         | 802.1Q tag/Vlan ID for vlan    | N/A         | N/A              |
|                    |               | being provisioned              |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| IntfList           | string        | List of interface names or     | N/A         | N/A              |
|                    |               | ifindex values to  be added as |             |                  |
|                    |               | tagged members of the vlan     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| UntagIntfList      | string        | List of interface names or     | N/A         | N/A              |
|                    |               | ifindex values to  be added as |             |                  |
|                    |               | untagged members of the vlan   |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+



**FlexSwitch CURL API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Vlan
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan<uuid>


**FlexSwitch SDK API Supported:**


- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getVlan(VlanId=vlanid)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **GET By ID**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getVlanById(ObjectId=objectid)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'




- **GET ALL**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getAllVlans()

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'




- **UPDATE**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.updateVlan(VlanId=vlanid, IntfList=intflist, UntagIntfList=untagintflist)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **UPDATE By ID**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.updateVlanById(ObjectId=objectidIntfList=intflist, UntagIntfList=untagintflist)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'
