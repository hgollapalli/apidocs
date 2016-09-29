FanSensorState Model Objects
============================================

*state/FanSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Fan Sensor Name.
	- This parameter is key element.
- **CurrentSpeed**
	- **Data Type**: int32
	- **Description**: Fan Current Speed.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/FanSensor


