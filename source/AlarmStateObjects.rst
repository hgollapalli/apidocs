AlarmState Model Objects
============================================

*state/Alarm*
------------------------------------

- Multiple of these objects can exist in a system.
- **EventName**
	- **Data Type**: string
	- **Description**: Alarm event name picked up from events.json.
	- This parameter is key element.
- **OwnerId**
	- **Data Type**: int32
	- **Description**: Alarm owner daemon Id picked up from events.json.
	- This parameter is key element.
- **OwnerName**
	- **Data Type**: string
	- **Description**: Alarm owner daemon name picked up from events.json.
	- This parameter is key element.
- **SrcObjName**
	- **Data Type**: string
	- **Description**: Alarm event name picked up from events.json.
	- This parameter is key element.
- **EventId**
	- **Data Type**: int32
	- **Description**: Alarm event id picked up from events.json.
	- This parameter is key element.
- **OccuranceTime**
	- **Data Type**: string
	- **Description**: Timestamp at which fault occured.
- **ResolutionTime**
	- **Data Type**: string
	- **Description**: Resolution Time stamp.
- **SrcObjKey**
	- **Data Type**: string
	- **Description**: Fault Object Key.
- **SrcObjUUID**
	- **Data Type**: string
	- **Description**: Fault Object UUID.
- **Description**
	- **Data Type**: string
	- **Description**: Description explaining the fault.
- **ResolutionReason**
	- **Data Type**: string
	- **Description**: Cleared/Disabled.
- **Severity**
	- **Data Type**: string
	- **Description**: Alarm Severity.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Alarm
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Alarm?CurrentMarker=<x>&Count=<y>


