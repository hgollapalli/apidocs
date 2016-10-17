PowerConverterSensorPMDataState Model Objects
=============================================================

*state/PowerConverterSensorPMData*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| **PARAMETER NAME** |       **DATA TYPE**        |       **DESCRIPTION**       | **DEFAULT** |     **VALID VALUES**      |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Class **[KEY]**    | string                     | Class of PM Data            | CLASS-A     | CLASS-A, CLASS-B, CLASS-B |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Name **[KEY]**     | string                     | Power Converter Sensor Name | N/A         | N/A                       |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Data               | PowerConverterSensorPMData |                             | N/A         | N/A                       |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+



**FlexSwitch CURL API Supported:**

	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData?CurrentMarker=<x>&Count=<y>


**FlexSwitch SDK API Supported:**


- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		fSwitch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = fSwitch.getPowerConverterSensorPMDataState(Class=class, Name=name)

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
		response, error = fSwitch.getPowerConverterSensorPMDataStateById(ObjectId=objectid)

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
		response, error = fSwitch.getAllPowerConverterSensorPMDataStates()

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


