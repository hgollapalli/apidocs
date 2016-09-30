XponderGlobal Model Objects
============================================

*config/XponderGlobal*
------------------------------------

- Only one of these object can exist in a system.
- **XponderId**
	- **Data Type**: uint8
	- **Description**: Xponder module identifier.
	- **Default**: 0
	- This parameter is key element.
- **XponderMode**
	- **Data Type**: string
	- **Description**: Global operational mode of Xponder module.
	- **Default**: OutOfService
- **XponderDescription**
	- **Data Type**: string
	- **Description**: User configurable description string for the xponder module.
	- **Default**: This is a Voyager platform


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/XponderGlobal
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/XponderGlobal/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/XponderGlobal
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/XponderGlobal<uuid>


