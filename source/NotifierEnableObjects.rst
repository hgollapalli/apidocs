NotifierEnable Model Objects
============================================

*config/NotifierEnable*
------------------------------------

- **Vrf**
	- **Data Type**: string
	- **Description**: Vrf name.
	- **Default**: default
	- This parameter is key element.
- **AlarmEnable**
	- **Data Type**: bool
	- **Description**: Enable Notifier.
	- **Default**: true
- **EventEnable**
	- **Data Type**: bool
	- **Description**: Enable Notifier.
	- **Default**: true
- **FaultEnable**
	- **Data Type**: bool
	- **Description**: Enable Notifier.
	- **Default**: true


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/NotifierEnable
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/NotifierEnable
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/NotifierEnable
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/NotifierEnable


