FMgrGlobal Model Objects
============================================

*config/FMgrGlobal*
------------------------------------

- **Vrf**
	- **Data Type**: string
	- **Description**: System Vrf.
	- **Default**: default
	- This parameter is key element.
- **Enable**
	- **Data Type**: bool
	- **Description**: Enable Fault Manager.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/FMgrGlobal
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/FMgrGlobal
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/FMgrGlobal
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/FMgrGlobal


