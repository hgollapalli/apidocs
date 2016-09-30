VoltageSensorState Model Objects
============================================

*state/VoltageSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Voltage Sensor Name.
	- This parameter is key element.
- **CurrentVoltage**
	- **Data Type**: float64
	- **Description**: Current Voltage Value.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/VoltageSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/VoltageSensor?CurrentMarker=<x>&Count=<y>


