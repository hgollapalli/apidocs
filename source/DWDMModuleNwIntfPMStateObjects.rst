DWDMModuleNwIntfPMState Model Objects
============================================

*state/DWDMModuleNwIntfPM*
------------------------------------

- Multiple of these objects can exist in a system.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **NwIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module network interface identifier.
	- This parameter is key element.
- **Resource**
	- **Data Type**: string
	- **Description**: Opticd resource name for which PM Data is required.
	- This parameter is key element.
- **Type**
	- **Data Type**: string
	- **Description**: Min/Max/Avg.
	- This parameter is key element.
- **Class**
	- **Data Type**: string
	- **Description**: Class of PM Data.
	- **Default**: CLASS-A
	- **Possible Values**: CLASS-A, CLASS-B, CLASS-B
	- This parameter is key element.
- **Data**
	- **Data Type**: DWDMModulePMData
	- **Description**: .


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntfPM
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntfPM?CurrentMarker=<x>&Count=<y>

