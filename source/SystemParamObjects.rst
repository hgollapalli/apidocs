SystemParam Model Objects
============================================

*config/SystemParam*
------------------------------------

- Multiple of these objects can exist in a system.
- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- **Default**: default
	- This parameter is key element.
- **SwitchMac**
	- **Data Type**: string
	- **Description**: Switch Mac Address.
- **Description**
	- **Data Type**: string
	- **Description**: System Description.
- **Hostname**
	- **Data Type**: string
	- **Description**: System Host Name.
- **MgmtIp**
	- **Data Type**: string
	- **Description**: Management Ip of System.
- **SwVersion**
	- **Data Type**: string
	- **Description**: FlexSwitch Version Information.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/SystemParam
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/SystemParam/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/SystemParam?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/SystemParam
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/SystemParam<uuid>


