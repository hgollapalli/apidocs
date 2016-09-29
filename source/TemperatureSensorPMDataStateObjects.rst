TemperatureSensorPMDataState Model Objects
============================================

*state/TemperatureSensorPMData*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Temperature Sensor Name.
	- This parameter is key element.
- **Class**
	- **Data Type**: string
	- **Description**: Class of PM Data.
	- **Default**: CLASS-A
	- **Possible Values**: CLASS-A, CLASS-B, CLASS-B
	- This parameter is key element.
- **Data**
	- **Data Type**: TemperatureSensorPMData
	- **Description**: .


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/TemperatureSensorPMData


