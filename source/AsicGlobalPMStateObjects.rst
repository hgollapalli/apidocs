AsicGlobalPMState Model Objects
============================================

*state/AsicGlobalPM*
------------------------------------

- Only one of these object can exist in a system.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: Module identifier.
	- This parameter is key element.
- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- This parameter is key element.
- **ClassAPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class A.
- **ClassBPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class B.
- **ClassCPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class C.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/AsicGlobalPM


