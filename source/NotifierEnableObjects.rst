NotifierEnable Model Objects
============================================

*config/NotifierEnable*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+-----------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** | **DESCRIPTION** | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+-----------------+-------------+------------------+
| Vrf **[KEY]**      | string        | Vrf name        | default     | N/A              |
+--------------------+---------------+-----------------+-------------+------------------+
| EventEnable        | bool          | Enable Notifier | true        | N/A              |
+--------------------+---------------+-----------------+-------------+------------------+
| FaultEnable        | bool          | Enable Notifier | true        | N/A              |
+--------------------+---------------+-----------------+-------------+------------------+
| AlarmEnable        | bool          | Enable Notifier | true        | N/A              |
+--------------------+---------------+-----------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/NotifierEnable
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/NotifierEnable/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/NotifierEnable
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/NotifierEnable<uuid>


