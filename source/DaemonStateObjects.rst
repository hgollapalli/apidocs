DaemonState Model Objects
============================================

*state/Daemon*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Name **[KEY]**     | string        | Daemon name                    | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| State              | string        | State of the daemon            | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| KeepAlive          | string        | KeepAlive state of the daemon  | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| RestartReason      | string        | Last restart reason            | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| RestartTime        | string        | Last restart time              | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| StartTime          | string        | Daemon start time              | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Enable             | bool          | If the daemon configured to be | N/A         | N/A              |
|                    |               | enabled                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Reason             | string        | Reason for current state of    | N/A         | N/A              |
|                    |               | the daemon                     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| RestartCount       | int32         | Number of times this daemon    | N/A         | N/A              |
|                    |               | has been restarted             |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Daemon
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Daemon?CurrentMarker=<x>&Count=<y>


