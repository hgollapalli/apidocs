PowerConverterSensorState Model Objects
============================================

*state/PowerConverterSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Power Converter Sensor Name.
	- This parameter is key element.
- **CurrentPower**
	- **Data Type**: float64
	- **Description**: Current Output Power Value.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/PowerConverterSensor


