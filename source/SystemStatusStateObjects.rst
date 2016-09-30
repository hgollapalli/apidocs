SystemStatusState Model Objects
============================================

*state/SystemStatus*
------------------------------------

- Only one of these object can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Name of the system.
	- This parameter is key element.
- **Reason**
	- **Data Type**: string
	- **Description**: Reason if system not ready.
- **UpTime**
	- **Data Type**: string
	- **Description**: Uptime of this system.
- **NumCreateCalls**
	- **Data Type**: string
	- **Description**: Number of create api calls made.
- **Ready**
	- **Data Type**: bool
	- **Description**: System is ready to accept api calls.
- **NumActionCalls**
	- **Data Type**: string
	- **Description**: Number of action api calls made.
- **NumDeleteCalls**
	- **Data Type**: string
	- **Description**: Number of delete api calls made.
- **NumGetCalls**
	- **Data Type**: string
	- **Description**: Number of get api calls made.
- **NumUpdateCalls**
	- **Data Type**: string
	- **Description**: Number of update api calls made.
- **FlexDaemons**
	- **Data Type**: DaemonState
	- **Description**: Daemon states.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/SystemStatus


