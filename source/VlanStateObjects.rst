VlanState Model Objects
============================================

*state/Vlan*
------------------------------------

- Multiple objects of this type can exist in a system.

+------------------------+---------------+--------------------------------+-------------+------------------+
|   **PARAMETER NAME**   | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VlanId **[KEY]**       | int32         | 802.1Q tag/Vlan ID for vlan    | N/A         | N/A              |
|                        |               | being provisioned              |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| IfIndex                | int32         | System assigned interface id   | N/A         | N/A              |
|                        |               | for this vlan interface        |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| OperState              | string        | Operational state of vlan      | N/A         | N/A              |
|                        |               | interface                      |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| SysInternalDescription | string        | This is a system generated     | N/A         | N/A              |
|                        |               | string that explains the       |             |                  |
|                        |               | operstate value                |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VlanName               | string        | System assigned vlan name      | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Vlan
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Vlan?CurrentMarker=<x>&Count=<y>


