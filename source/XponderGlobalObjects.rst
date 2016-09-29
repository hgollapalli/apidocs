XponderGlobal Model Objects
============================================

*config/XponderGlobal*
------------------------------------

- **XponderId**
	- **Data Type**: uint8
	- **Description**: Xponder module identifier.
	- **Default**: 0
	- This parameter is key element.
- **XponderDescription**
	- **Data Type**: string
	- **Description**: User configurable description string for the xponder module.
	- **Default**: This is a Voyager platform
- **XponderMode**
	- **Data Type**: string
	- **Description**: Global operational mode of Xponder module.
	- **Default**: OutOfService


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/XponderGlobal
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/XponderGlobal
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/XponderGlobal
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/XponderGlobal


