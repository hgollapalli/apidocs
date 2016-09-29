DWDMModule Model Objects
============================================

*config/DWDMModule*
------------------------------------

- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **PMInterval**
	- **Data Type**: uint8
	- **Description**: Performance monitoring interval.
	- **Default**: 1
- **AdminState**
	- **Data Type**: string
	- **Description**: Reset state of this dwdm module (false (Reset deasserted).
	- **Default**: DOWN
- **EnableExtPMTickSrc**
	- **Data Type**: bool
	- **Description**: Enable/Disable external tick source for performance monitoring.
	- **Default**: false
- **IndependentLaneMode**
	- **Data Type**: bool
	- **Description**: Network lane configuration for the DWDM Module. true-Independent lanes.
	- **Default**: true


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/DWDMModule
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/DWDMModule


