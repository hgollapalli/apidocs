SystemStatusState Model Objects
============================================

*state/SystemStatus*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Name of the system.
	- This parameter is key element.
- **NumUpdateCalls**
	- **Data Type**: string
	- **Description**: Number of update api calls made.
- **NumCreateCalls**
	- **Data Type**: string
	- **Description**: Number of create api calls made.
- **NumDeleteCalls**
	- **Data Type**: string
	- **Description**: Number of delete api calls made.
- **NumGetCalls**
	- **Data Type**: string
	- **Description**: Number of get api calls made.
- **Ready**
	- **Data Type**: bool
	- **Description**: System is ready to accept api calls.
- **Reason**
	- **Data Type**: string
	- **Description**: Reason if system not ready.
- **FlexDaemons**
	- **Data Type**: DaemonState
	- **Description**: Daemon states.
- **NumActionCalls**
	- **Data Type**: string
	- **Description**: Number of action api calls made.
- **UpTime**
	- **Data Type**: string
	- **Description**: Uptime of this system.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/SystemStatus


