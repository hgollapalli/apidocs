AsicGlobalState Model Objects
============================================

*state/AsicGlobal*
------------------------------------

- Only one of these object can exist in a system.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: Module identifier.
	- This parameter is key element.
- **ModuleTemp**
	- **Data Type**: float64
	- **Description**: Current module temperature.
- **PartNumber**
	- **Data Type**: string
	- **Description**: Part number of underlying switching asic.
- **RevisionId**
	- **Data Type**: string
	- **Description**: Revision ID of underlying switching asic.
- **VendorId**
	- **Data Type**: string
	- **Description**: Vendor identification value.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/AsicGlobal


