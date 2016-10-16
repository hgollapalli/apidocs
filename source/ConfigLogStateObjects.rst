ConfigLogState Model Objects
============================================

*state/ConfigLog*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| API **[KEY]**      | string        | Name of the API called         | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| SeqNum **[KEY]**   | uint32        | Sequence number of the API     | N/A         | N/A              |
|                    |               | call                           |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Time **[KEY]**     | string        | When the API was called        | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| UserAddr           | string        | Host address from where the    | N/A         | N/A              |
|                    |               | call was made                  |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| UserName           | string        | User who made the call         | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Data               | string        | User provided data             | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Operation          | string        | Oprtation executed on this API | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Result             | string        | Result of the API call         | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/ConfigLog
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/ConfigLog?CurrentMarker=<x>&Count=<y>


