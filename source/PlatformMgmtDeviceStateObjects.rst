PlatformMgmtDeviceState Model Objects
============================================

*state/PlatformMgmtDevice*
------------------------------------

- Only one of these object can exist in a system.
- **DeviceName**
	- **Data Type**: string
	- **Description**: Device Name.
	- **Default**: BMC
	- This parameter is key element.
- **CPUUsage**
	- **Data Type**: string
	- **Description**: CPU Usage.
- **Description**
	- **Data Type**: string
	- **Description**: Platform Description.
- **MemoryUsage**
	- **Data Type**: string
	- **Description**: Memory Usage.
- **ResetReason**
	- **Data Type**: string
	- **Description**: Reset Reason.
- **Uptime**
	- **Data Type**: string
	- **Description**: Uptime and load description.
- **Version**
	- **Data Type**: string
	- **Description**: Version.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PlatformMgmtDevice


