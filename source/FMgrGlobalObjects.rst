FMgrGlobal Model Objects
============================================

*config/FMgrGlobal*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+----------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |   **DESCRIPTION**    | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+----------------------+-------------+------------------+
| Vrf **[KEY]**      | string        | System Vrf           | default     | N/A              |
+--------------------+---------------+----------------------+-------------+------------------+
| Enable             | bool          | Enable Fault Manager | N/A         | N/A              |
+--------------------+---------------+----------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FMgrGlobal
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/FMgrGlobal/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FMgrGlobal
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FMgrGlobal<uuid>


