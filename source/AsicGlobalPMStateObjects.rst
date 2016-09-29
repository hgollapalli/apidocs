AsicGlobalPMState Model Objects
============================================

*state/AsicGlobalPM*
------------------------------------

- **ModuleId**
	- **Data Type**: uint8
	- **Description**: Module identifier.
	- This parameter is key element.
- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- This parameter is key element.
- **ClassCPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class C.
- **ClassAPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class A.
- **ClassBPMData**
	- **Data Type**: PMData
	- **Description**: PM Data corresponding to PM Class B.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/AsicGlobalPM


