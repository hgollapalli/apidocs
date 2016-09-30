FanSensorState Model Objects
============================================

*state/FanSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Fan Sensor Name.
	- This parameter is key element.
- **CurrentSpeed**
	- **Data Type**: int32
	- **Description**: Fan Current Speed.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/FanSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/FanSensor?CurrentMarker=<x>&Count=<y>


