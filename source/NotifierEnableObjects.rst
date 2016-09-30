NotifierEnable Model Objects
============================================

*config/NotifierEnable*
------------------------------------

- Only one of these object can exist in a system.
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


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/NotifierEnable
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/NotifierEnable/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/NotifierEnable
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/NotifierEnable<uuid>


