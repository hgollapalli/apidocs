FanSensor Model Objects
=============================================================

*config/FanSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+------------------------+---------------+--------------------------------+-------------+------------------+
|   **PARAMETER NAME**   | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+------------------------+---------------+--------------------------------+-------------+------------------+
| Name **[KEY]**         | string        | Fan Sensor Name                | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| AdminState             | string        | Enable/Disable                 | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState     | string        | PM Class-A Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState     | string        | PM Class-B Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmThreshold   | int32         | Higher Alarm Threshold for TCA | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningThreshold | int32         | Higher Warning Threshold for   | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmThreshold    | int32         | Lower Alarm Threshold for TCA  | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningThreshold  | int32         | Lower Warning Threshold for    | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState     | string        | PM Class-C Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+



**FlexSwitch CURL API Supported:**

	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FanSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor?CurrentMarker=<x>&Count=<y>
	- CREATE(POST)
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FanSensor
	- DELETE By Key
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1/config/FanSensor
	- DELETE By ID
		 curl -X DELETE http://device-management-IP:8080/public/v1/config/FanSensor<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor<uuid>


**FlexSwitch SDK API Supported:**


- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.getFanSensor(Name=name)

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
		response, error = fSwitch.getFanSensorById(ObjectId=objectid)

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
		response, error = fSwitch.getAllFanSensors()

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.createFanSensor(Name=name, AdminState=adminstate, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, HigherAlarmThreshold=higheralarmthreshold, HigherWarningThreshold=higherwarningthreshold, LowerAlarmThreshold=loweralarmthreshold, LowerWarningThreshold=lowerwarningthreshold, PMClassCAdminState=pmclasscadminstate)

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.deleteFanSensor(Name=name)

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.deleteFanSensorById(ObjectId=objectid

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.updateFanSensor(Name=name, AdminState=adminstate, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, HigherAlarmThreshold=higheralarmthreshold, HigherWarningThreshold=higherwarningthreshold, LowerAlarmThreshold=loweralarmthreshold, LowerWarningThreshold=lowerwarningthreshold, PMClassCAdminState=pmclasscadminstate)

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
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.updateFanSensorById(ObjectId=objectidAdminState=adminstate, PMClassAAdminState=pmclassaadminstate, PMClassBAdminState=pmclassbadminstate, HigherAlarmThreshold=higheralarmthreshold, HigherWarningThreshold=higherwarningthreshold, LowerAlarmThreshold=loweralarmthreshold, LowerWarningThreshold=lowerwarningthreshold, PMClassCAdminState=pmclasscadminstate)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'
