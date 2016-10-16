SystemStatusState Model Objects
============================================

*state/SystemStatus*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Name **[KEY]**     | string        | Name of the system             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| NumActionCalls     | string        | Number of action api calls     | N/A         | N/A              |
|                    |               | made                           |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| NumDeleteCalls     | string        | Number of delete api calls     | N/A         | N/A              |
|                    |               | made                           |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| NumGetCalls        | string        | Number of get api calls made   | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| NumUpdateCalls     | string        | Number of update api calls     | N/A         | N/A              |
|                    |               | made                           |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Ready              | bool          | System is ready to accept api  | N/A         | N/A              |
|                    |               | calls                          |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Reason             | string        | Reason if system not ready     | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| FlexDaemons        | DaemonState   | Daemon states                  | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| NumCreateCalls     | string        | Number of create api calls     | N/A         | N/A              |
|                    |               | made                           |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| UpTime             | string        | Uptime of this system          | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/SystemStatus


