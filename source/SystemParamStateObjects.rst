SystemParamState Model Objects
============================================

*state/SystemParam*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Vrf **[KEY]**      | string        | System Vrf                     | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Description        | string        | System Description             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Distro             | string        | Linux distro running on this   | N/A         | N/A              |
|                    |               | system                         |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Hostname           | string        | System Host Name               | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Kernel             | string        | Kernel version running on this | N/A         | N/A              |
|                    |               | system                         |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| MgmtIp             | string        | Management Ip of System        | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| SwVersion          | string        | FlexSwitch Version Information | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| SwitchMac          | string        | Switch Mac Address             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/SystemParam
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/SystemParam?CurrentMarker=<x>&Count=<y>


