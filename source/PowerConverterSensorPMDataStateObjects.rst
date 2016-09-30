PowerConverterSensorPMDataState Model Objects
============================================

*state/PowerConverterSensorPMData*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Power Converter Sensor Name.
	- This parameter is key element.
- **Class**
	- **Data Type**: string
	- **Description**: Class of PM Data.
	- **Default**: CLASS-A
	- **Possible Values**: CLASS-A, CLASS-B, CLASS-B
	- This parameter is key element.
- **Data**
	- **Data Type**: PowerConverterSensorPMData
	- **Description**: .


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData?CurrentMarker=<x>&Count=<y>


