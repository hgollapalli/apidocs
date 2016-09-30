FaultState Model Objects
============================================

*state/Fault*
------------------------------------

- Multiple of these objects can exist in a system.
- **OwnerName**
	- **Data Type**: string
	- **Description**: Fault owner daemon name picked up from events.json.
	- This parameter is key element.
- **OwnerId**
	- **Data Type**: int32
	- **Description**: Fault owner daemon Id picked up from events.json.
	- This parameter is key element.
- **SrcObjName**
	- **Data Type**: string
	- **Description**: Fault event name picked up from events.json.
	- This parameter is key element.
- **EventId**
	- **Data Type**: int32
	- **Description**: Fault event id picked up from events.json.
	- This parameter is key element.
- **EventName**
	- **Data Type**: string
	- **Description**: Fault event name picked up from events.json.
	- This parameter is key element.
- **SrcObjKey**
	- **Data Type**: string
	- **Description**: Fault Object Key.
- **ResolutionReason**
	- **Data Type**: string
	- **Description**: Cleared/Disabled.
- **ResolutionTime**
	- **Data Type**: string
	- **Description**: Resolution Time stamp.
- **Description**
	- **Data Type**: string
	- **Description**: Description explaining the fault.
- **OccuranceTime**
	- **Data Type**: string
	- **Description**: Timestamp at which fault occured.
- **SrcObjUUID**
	- **Data Type**: string
	- **Description**: Fault Object UUID.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Fault
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Fault?CurrentMarker=<x>&Count=<y>


