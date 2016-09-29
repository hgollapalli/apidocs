DaemonState Model Objects
============================================

*state/Daemon*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Daemon name.
	- This parameter is key element.
- **Enable**
	- **Data Type**: bool
	- **Description**: If the daemon configured to be enabled.
- **KeepAlive**
	- **Data Type**: string
	- **Description**: KeepAlive state of the daemon.
- **RestartTime**
	- **Data Type**: string
	- **Description**: Last restart time.
- **Reason**
	- **Data Type**: string
	- **Description**: Reason for current state of the daemon.
- **RestartCount**
	- **Data Type**: int32
	- **Description**: Number of times this daemon has been restarted.
- **RestartReason**
	- **Data Type**: string
	- **Description**: Last restart reason.
- **StartTime**
	- **Data Type**: string
	- **Description**: Daemon start time.
- **State**
	- **Data Type**: string
	- **Description**: State of the daemon.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/Daemon


