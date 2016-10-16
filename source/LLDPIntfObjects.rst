LLDPIntf Model Objects
============================================

*config/LLDPIntf*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+----------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** |   **VALID VALUES**   |
+--------------------+---------------+--------------------------------+-------------+----------------------+
| IntfRef **[KEY]**  | string        | IfIndex where lldp needs is    | None        | N/A                  |
|                    |               | enabled/disabled               |             |                      |
+--------------------+---------------+--------------------------------+-------------+----------------------+
| TxRxMode           | string        | Transmit/Receive mode          | TxRx        | TxOnly, RxOnly, TxRx |
|                    |               | configruration for the LLDP    |             |                      |
|                    |               | agent specific to an interface |             |                      |
+--------------------+---------------+--------------------------------+-------------+----------------------+
| Enable             | bool          | Enable/Disable lldp config Per | true        | N/A                  |
|                    |               | Port                           |             |                      |
+--------------------+---------------+--------------------------------+-------------+----------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/LLDPIntf
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/LLDPIntf/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/LLDPIntf?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/LLDPIntf
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/LLDPIntf<uuid>


