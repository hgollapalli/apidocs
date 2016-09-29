VoltageSensorState Model Objects
============================================

*state/VoltageSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Voltage Sensor Name.
	- This parameter is key element.
- **CurrentVoltage**
	- **Data Type**: float64
	- **Description**: Current Voltage Value.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/VoltageSensor


