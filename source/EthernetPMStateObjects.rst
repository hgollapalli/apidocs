EthernetPMState Model Objects
============================================

*state/EthernetPM*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| IntfRef **[KEY]**  | string        | Interface name of port         | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Resource **[KEY]** | string        | Resource identifier            | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassCPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class C                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassAPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class A                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassBPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class B                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/EthernetPM
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/EthernetPM?CurrentMarker=<x>&Count=<y>


