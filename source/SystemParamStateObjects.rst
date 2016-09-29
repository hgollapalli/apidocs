SystemParamState Model Objects
============================================

*state/SystemParam*
------------------------------------

- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- This parameter is key element.
- **Description**
	- **Data Type**: string
	- **Description**: System Description.
- **Distro**
	- **Data Type**: string
	- **Description**: Linux distro running on this system.
- **Hostname**
	- **Data Type**: string
	- **Description**: System Host Name.
- **Kernel**
	- **Data Type**: string
	- **Description**: Kernel version running on this system.
- **MgmtIp**
	- **Data Type**: string
	- **Description**: Management Ip of System.
- **SwVersion**
	- **Data Type**: string
	- **Description**: FlexSwitch Version Information.
- **SwitchMac**
	- **Data Type**: string
	- **Description**: Switch Mac Address.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/SystemParam


