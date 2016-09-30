SystemParamState Model Objects
============================================

*state/SystemParam*
------------------------------------

- Multiple of these objects can exist in a system.
- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- This parameter is key element.
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
- **Description**
	- **Data Type**: string
	- **Description**: System Description.
- **Distro**
	- **Data Type**: string
	- **Description**: Linux distro running on this system.
- **Hostname**
	- **Data Type**: string
	- **Description**: System Host Name.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/SystemParam
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/SystemParam?CurrentMarker=<x>&Count=<y>


