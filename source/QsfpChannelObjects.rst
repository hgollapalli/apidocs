QsfpChannel Model Objects
=============================================================

*config/QsfpChannel*
------------------------------------

- Multiple objects of this type can exist in a system.

+----------------------+---------------+--------------------------------+-------------+------------------+
|  **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+----------------------+---------------+--------------------------------+-------------+------------------+
| QsfpId **[KEY]**     | int32         | Qsfp Id                        | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| ChannelNum **[KEY]** | int32         | Qsfp Channel Number            | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmTXBias    | float64       | Higher Alarm Tx Current Bias   | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningRXPower | float64       | Higher Warning Rx power        | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningTXBias  | float64       | Higher Warning Tx Current Bias | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmTXBias     | float64       | Lower Alarm Tx Current Bias    | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmRXPower   | float64       | Higher Alarm Rx power          | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmTXPower   | float64       | Higher Alarm Rx power for TCA  | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningTXPower  | float64       | Lower Warning Rx power for TCA | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState   | string        | PM Class-C Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmTXPower    | float64       | Lower Alarm Rx power for TCA   | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningRXPower  | float64       | Lower Warning Rx power         | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState   | string        | PM Class-A Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState   | string        | PM Class-B Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningTXBias   | float64       | Lower Warning Tx Current Bias  | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| AdminState           | string        | Enable/Disable                 | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningTXPower | float64       | Higher Warning Rx power for    | N/A         | N/A              |
|                      |               | TCA                            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmRXPower    | float64       | Lower Alarm Rx power Threshold | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+



**FlexSwitch CURL API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/QsfpChannel
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel?CurrentMarker=<x>&Count=<y>
	- CREATE(POST)
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/QsfpChannel
	- DELETE By Key
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1/config/QsfpChannel
	- DELETE By ID
		 curl -X DELETE http://device-management-IP:8080/public/v1/config/QsfpChannel<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel<uuid>


**FlexSwitch SDK API Supported:**


- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getQsfpChannel(QsfpId=qsfpid, ChannelNum=channelnum)

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
		response, error = swtch.getQsfpChannelById(ObjectId=objectid)

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
		response, error = swtch.getAllQsfpChannels()

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **CREATE**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.createQsfpChannel(QsfpId=qsfpid, ChannelNum=channelnum, HigherAlarmTXBias=higheralarmtxbias, HigherWarningRXPower=higherwarningrxpower, HigherWarningTXBias=higherwarningtxbias, LowerAlarmTXBias=loweralarmtxbias, HigherAlarmRXPower=higheralarmrxpower, HigherAlarmTXPower=higheralarmtxpower, LowerWarningTXPower=lowerwarningtxpower, PMClassCAdminState=pmclasscadminstate, LowerAlarmTXPower=loweralarmtxpower, LowerWarningRXPower=lowerwarningrxpower, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, LowerWarningTXBias=lowerwarningtxbias, AdminState=adminstate, HigherWarningTXPower=higherwarningtxpower, LowerAlarmRXPower=loweralarmrxpower)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **DELETE**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.deleteQsfpChannel(QsfpId=qsfpid, ChannelNum=channelnum)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **DELETE By ID**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.deleteQsfpChannelById(ObjectId=objectid

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
		response, error = swtch.updateQsfpChannel(QsfpId=qsfpid, ChannelNum=channelnum, HigherAlarmTXBias=higheralarmtxbias, HigherWarningRXPower=higherwarningrxpower, HigherWarningTXBias=higherwarningtxbias, LowerAlarmTXBias=loweralarmtxbias, HigherAlarmRXPower=higheralarmrxpower, HigherAlarmTXPower=higheralarmtxpower, LowerWarningTXPower=lowerwarningtxpower, PMClassCAdminState=pmclasscadminstate, LowerAlarmTXPower=loweralarmtxpower, LowerWarningRXPower=lowerwarningrxpower, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, LowerWarningTXBias=lowerwarningtxbias, AdminState=adminstate, HigherWarningTXPower=higherwarningtxpower, LowerAlarmRXPower=loweralarmrxpower)

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
		response, error = swtch.updateQsfpChannelById(ObjectId=objectidHigherAlarmTXBias=higheralarmtxbias, HigherWarningRXPower=higherwarningrxpower, HigherWarningTXBias=higherwarningtxbias, LowerAlarmTXBias=loweralarmtxbias, HigherAlarmRXPower=higheralarmrxpower, HigherAlarmTXPower=higheralarmtxpower, LowerWarningTXPower=lowerwarningtxpower, PMClassCAdminState=pmclasscadminstate, LowerAlarmTXPower=loweralarmtxpower, LowerWarningRXPower=lowerwarningrxpower, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, LowerWarningTXBias=lowerwarningtxbias, AdminState=adminstate, HigherWarningTXPower=higherwarningtxpower, LowerAlarmRXPower=loweralarmrxpower)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'
