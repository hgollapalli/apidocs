SystemParam Model Objects
============================================

*config/SystemParam*
------------------------------------

- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- **Default**: default
	- This parameter is key element.
- **Hostname**
	- **Data Type**: string
	- **Description**: System Host Name.
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


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/SystemParam
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/SystemParam
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/SystemParam
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/SystemParam


