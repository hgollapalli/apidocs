SystemParam Model Objects
============================================

*config/SystemParam*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Vrf **[KEY]**      | string        | System Vrf                     | default     | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Hostname           | string        | System Host Name               | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| MgmtIp             | string        | Management Ip of System        | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| SwVersion          | string        | FlexSwitch Version Information | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| SwitchMac          | string        | Switch Mac Address             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Description        | string        | System Description             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/SystemParam
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/SystemParam/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/SystemParam?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/SystemParam
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/SystemParam<uuid>


