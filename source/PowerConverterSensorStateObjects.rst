PowerConverterSensorState Model Objects
============================================

*state/PowerConverterSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Power Converter Sensor Name.
	- This parameter is key element.
- **CurrentPower**
	- **Data Type**: float64
	- **Description**: Current Output Power Value.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PowerConverterSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/PowerConverterSensor?CurrentMarker=<x>&Count=<y>


