TemperatureSensorState Model Objects
============================================

*state/TemperatureSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Temperature Sensor Name.
	- This parameter is key element.
- **CurrentTemperature**
	- **Data Type**: float64
	- **Description**: Current Temperature Value.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/TemperatureSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/TemperatureSensor?CurrentMarker=<x>&Count=<y>


