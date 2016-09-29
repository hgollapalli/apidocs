XponderGlobalState Model Objects
============================================

*state/XponderGlobal*
------------------------------------

- **XponderId**
	- **Data Type**: uint8
	- **Description**: Xponder module identifier.
	- This parameter is key element.
- **XponderDescription**
	- **Data Type**: string
	- **Description**: User configurable description string for the xponder module.
- **XponderMode**
	- **Data Type**: string
	- **Description**: Global operational mode of Xponder module.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/XponderGlobal


