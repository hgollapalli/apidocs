MacTableEntryState Model Objects
============================================

*state/MacTableEntry*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| MacAddr **[KEY]**  | string        | MAC Address                    | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Port               | int32         | Port number on which mac was   |           0 | N/A              |
|                    |               | learned                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| VlanId             | int32         | Vlan id corresponding to which |           0 | N/A              |
|                    |               | mac was learned                |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/MacTableEntry


