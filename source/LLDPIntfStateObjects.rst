LLDPIntfState Model Objects
=============================================================

*state/LLDPIntf*
------------------------------------

- Multiple objects of this type can exist in a system.

+---------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+---------------------+---------------+--------------------------------+-------------+------------------+
| IntfRef **[KEY]**   | string        | IntfRef where lldp is          | N/A         | N/A              |
|                     |               | configured                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerMac             | string        | Mac address of direct          | N/A         | N/A              |
|                     |               | connection                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SendFrames          | int32         | Total Frames send to the       | N/A         | N/A              |
|                     |               | neighbor                       |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SystemCapabilities  | string        | System Capabilities of the     | N/A         | N/A              |
|                     |               | peer port                      |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| Enable              | bool          | Enable/Disable lldp config     | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| LocalPort           | string        | Local interface                | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerHostName        | string        | Name of the peer host          | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| ReceivedFrames      | int32         | Total Frames received from     | N/A         | N/A              |
|                     |               | neighbor                       |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SystemDescription   | string        | System Description of the peer | N/A         | N/A              |
|                     |               | port                           |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| EnabledCapabilities | string        | Enabled Capabilities of the    | N/A         | N/A              |
|                     |               | peer port                      |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| HoldTime            | string        | Validity of the peer           | N/A         | N/A              |
|                     |               | information                    |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| IfIndex             | int32         | IfIndex where lldp needs to be | N/A         | N/A              |
|                     |               | configured                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerPort            | string        | Name of directtly connected    | N/A         | N/A              |
|                     |               | pors                           |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+



**FlexSwitch CURL API Supported:**

	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/LLDPIntf
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/LLDPIntf?CurrentMarker=<x>&Count=<y>


**FlexSwitch SDK API Supported:**


- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.getLLDPIntfState(IntfRef=intfref)

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.getLLDPIntfStateById(ObjectId=objectid)

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.getAllLLDPIntfStates()

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


