FaultState Model Objects
============================================

*state/Fault*
------------------------------------

- Multiple objects of this type can exist in a system.

+----------------------+---------------+--------------------------------+-------------+------------------+
|  **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+----------------------+---------------+--------------------------------+-------------+------------------+
| EventId **[KEY]**    | int32         | Fault event id picked up from  | N/A         | N/A              |
|                      |               | events.json                    |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| OwnerId **[KEY]**    | int32         | Fault owner daemon Id picked   | N/A         | N/A              |
|                      |               | up from events.json            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| OwnerName **[KEY]**  | string        | Fault owner daemon name picked | N/A         | N/A              |
|                      |               | up from events.json            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| SrcObjName **[KEY]** | string        | Fault event name picked up     | N/A         | N/A              |
|                      |               | from events.json               |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| EventName **[KEY]**  | string        | Fault event name picked up     | N/A         | N/A              |
|                      |               | from events.json               |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| OccuranceTime        | string        | Timestamp at which fault       | N/A         | N/A              |
|                      |               | occured                        |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| ResolutionReason     | string        | Cleared/Disabled               | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| ResolutionTime       | string        | Resolution Time stamp          | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| SrcObjKey            | string        | Fault Object Key               | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| Description          | string        | Description explaining the     | N/A         | N/A              |
|                      |               | fault                          |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| SrcObjUUID           | string        | Fault Object UUID              | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Fault
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Fault?CurrentMarker=<x>&Count=<y>


