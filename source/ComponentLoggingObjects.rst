ComponentLogging Model Objects
============================================

*config/ComponentLogging*
------------------------------------

- Multiple of these objects can exist in a system.
- **Module**
	- **Data Type**: string
	- **Description**: Module name to set logging level.
	- This parameter is key element.
- **Level**
	- **Data Type**: string
	- **Description**: Logging level.
	- **Default**: info


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/ComponentLogging
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/ComponentLogging/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/ComponentLogging?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/ComponentLogging
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/ComponentLogging<uuid>


