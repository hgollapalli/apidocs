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
| LowerAlarmTXBias     | float64       | Lower Alarm Tx Current Bias    | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState   | string        | PM Class-A Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState   | string        | PM Class-C Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmTXPower   | float64       | Higher Alarm Rx power for TCA  | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningRXPower | float64       | Higher Warning Rx power        | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningTXPower | float64       | Higher Warning Rx power for    | N/A         | N/A              |
|                      |               | TCA                            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningTXPower  | float64       | Lower Warning Rx power for TCA | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState   | string        | PM Class-B Admin State         | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmTXBias    | float64       | Higher Alarm Tx Current Bias   | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningTXBias  | float64       | Higher Warning Tx Current Bias | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningRXPower  | float64       | Lower Warning Rx power         | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningTXBias   | float64       | Lower Warning Tx Current Bias  | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| AdminState           | string        | Enable/Disable                 | Disable     | Enable, Disable  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmRXPower   | float64       | Higher Alarm Rx power          | N/A         | N/A              |
|                      |               | Threshold for TCA              |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmRXPower    | float64       | Lower Alarm Rx power Threshold | N/A         | N/A              |
|                      |               | for TCA                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmTXPower    | float64       | Lower Alarm Rx power for TCA   | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+



*FlexSwitch CURL API Supported*
------------------------------------

	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/QsfpChannel
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel<uuid>


*FlexSwitch SDK API Supported:*
------------------------------------



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




- **UPDATE**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.updateQsfpChannel(QsfpId=qsfpid, ChannelNum=channelnum, LowerAlarmTXBias=loweralarmtxbias, PMClassAAdminState=pmclassaadminstate, PMClassCAdminState=pmclasscadminstate, HigherAlarmTXPower=higheralarmtxpower, HigherWarningRXPower=higherwarningrxpower, HigherWarningTXPower=higherwarningtxpower, LowerWarningTXPower=lowerwarningtxpower, PMClassBAdminState=pmclassbadminstate, HigherAlarmTXBias=higheralarmtxbias, HigherWarningTXBias=higherwarningtxbias, LowerWarningRXPower=lowerwarningrxpower, LowerWarningTXBias=lowerwarningtxbias, AdminState=adminstate, HigherAlarmRXPower=higheralarmrxpower, LowerAlarmRXPower=loweralarmrxpower, LowerAlarmTXPower=loweralarmtxpower)

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
		response, error = swtch.updateQsfpChannelById(ObjectId=objectidLowerAlarmTXBias=loweralarmtxbias, PMClassAAdminState=pmclassaadminstate, PMClassCAdminState=pmclasscadminstate, HigherAlarmTXPower=higheralarmtxpower, HigherWarningRXPower=higherwarningrxpower, HigherWarningTXPower=higherwarningtxpower, LowerWarningTXPower=lowerwarningtxpower, PMClassBAdminState=pmclassbadminstate, HigherAlarmTXBias=higheralarmtxbias, HigherWarningTXBias=higherwarningtxbias, LowerWarningRXPower=lowerwarningrxpower, LowerWarningTXBias=lowerwarningtxbias, AdminState=adminstate, HigherAlarmRXPower=higheralarmrxpower, LowerAlarmRXPower=loweralarmrxpower, LowerAlarmTXPower=loweralarmtxpower)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'
