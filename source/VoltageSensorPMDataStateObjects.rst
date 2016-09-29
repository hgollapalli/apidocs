VoltageSensorPMDataState Model Objects
============================================

*state/VoltageSensorPMData*
------------------------------------

- **Class**
	- **Data Type**: string
	- **Description**: Class of PM Data.
	- **Default**: CLASS-A
	- **Possible Values**: CLASS-A, CLASS-B, CLASS-B
	- This parameter is key element.
- **Name**
	- **Data Type**: string
	- **Description**: Voltage Sensor Name.
	- This parameter is key element.
- **Data**
	- **Data Type**: VoltageSensorPMData
	- **Description**: .


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/VoltageSensorPMData


