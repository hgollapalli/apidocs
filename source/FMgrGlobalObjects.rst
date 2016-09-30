FMgrGlobal Model Objects
============================================

*config/FMgrGlobal*
------------------------------------

- Only one of these object can exist in a system.
- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- **Default**: default
	- This parameter is key element.
- **Enable**
	- **Data Type**: bool
	- **Description**: Enable Fault Manager.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FMgrGlobal
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/FMgrGlobal/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FMgrGlobal
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FMgrGlobal<uuid>


