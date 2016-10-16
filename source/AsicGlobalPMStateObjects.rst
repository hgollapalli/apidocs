AsicGlobalPMState Model Objects
============================================

*state/AsicGlobalPM*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]** | uint8         | Module identifier              | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Resource **[KEY]** | string        | Resource identifier            | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassBPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class B                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassCPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class C                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ClassAPMData       | PMData        | PM Data corresponding to PM    | N/A         | N/A              |
|                    |               | Class A                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/AsicGlobalPM


