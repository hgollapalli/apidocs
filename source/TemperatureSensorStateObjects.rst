TemperatureSensorState Model Objects
============================================

*state/TemperatureSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Temperature Sensor Name.
	- This parameter is key element.
- **CurrentTemperature**
	- **Data Type**: float64
	- **Description**: Current Temperature Value.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/TemperatureSensor


