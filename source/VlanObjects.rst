Vlan Model Objects
============================================

*config/Vlan*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| VlanId **[KEY]**   | int32         | 802.1Q tag/Vlan ID for vlan    | N/A         | N/A              |
|                    |               | being provisioned              |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| IntfList           | string        | List of interface names or     | N/A         | N/A              |
|                    |               | ifindex values to  be added as |             |                  |
|                    |               | tagged members of the vlan     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| UntagIntfList      | string        | List of interface names or     | N/A         | N/A              |
|                    |               | ifindex values to  be added as |             |                  |
|                    |               | untagged members of the vlan   |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| AdminState         | string        | Administrative state of this   | UP          | UP, DOWN         |
|                    |               | vlan interface                 |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Vlan
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan<uuid>


