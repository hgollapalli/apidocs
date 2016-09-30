DaemonState Model Objects
============================================

*state/Daemon*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Daemon name.
	- This parameter is key element.
- **Reason**
	- **Data Type**: string
	- **Description**: Reason for current state of the daemon.
- **RestartReason**
	- **Data Type**: string
	- **Description**: Last restart reason.
- **State**
	- **Data Type**: string
	- **Description**: State of the daemon.
- **Enable**
	- **Data Type**: bool
	- **Description**: If the daemon configured to be enabled.
- **KeepAlive**
	- **Data Type**: string
	- **Description**: KeepAlive state of the daemon.
- **RestartCount**
	- **Data Type**: int32
	- **Description**: Number of times this daemon has been restarted.
- **RestartTime**
	- **Data Type**: string
	- **Description**: Last restart time.
- **StartTime**
	- **Data Type**: string
	- **Description**: Daemon start time.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Daemon
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Daemon?CurrentMarker=<x>&Count=<y>


