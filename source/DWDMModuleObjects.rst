DWDMModule Model Objects
============================================

*config/DWDMModule*
------------------------------------

- Multiple of these objects can exist in a system.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
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
- **PMInterval**
	- **Data Type**: uint8
	- **Description**: Performance monitoring interval.
	- **Default**: 1


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/DWDMModule
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModule/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModule?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModule
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModule<uuid>


