XponderGlobalState Model Objects
============================================

*state/XponderGlobal*
------------------------------------

- Only one object of this type can exist in a system.

+---------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+---------------------+---------------+--------------------------------+-------------+------------------+
| XponderId **[KEY]** | uint8         | Xponder module identifier      | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| XponderMode         | string        | Global operational mode of     | N/A         | N/A              |
|                     |               | Xponder module                 |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| XponderDescription  | string        | User configurable description  | N/A         | N/A              |
|                     |               | string for the xponder module  |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/XponderGlobal


