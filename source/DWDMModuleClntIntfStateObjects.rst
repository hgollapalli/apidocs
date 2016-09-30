DWDMModuleClntIntfState Model Objects
============================================

*state/DWDMModuleClntIntf*
------------------------------------

- Multiple of these objects can exist in a system.
- **ClntIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module client interface identifier.
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **PRBSTxErrCntLane0**
	- **Data Type**: float64
	- **Description**: Client interface host lane 0 PRBS TX Error count.
- **PRBSTxErrCntLane1**
	- **Data Type**: float64
	- **Description**: Client interface host lane 1 PRBS TX Error count.
- **PRBSTxErrCntLane2**
	- **Data Type**: float64
	- **Description**: Client interface host lane 2 PRBS TX Error count.
- **PRBSTxErrCntLane3**
	- **Data Type**: float64
	- **Description**: Client interface host lane 3 PRBS TX Error count.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModuleClntIntf
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModuleClntIntf?CurrentMarker=<x>&Count=<y>


