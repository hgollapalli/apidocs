ApiInfoState Model Objects
============================================

*state/ApiInfo*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Url **[KEY]**      | string        | URL                            | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Info               | string        | APIs available under this URL  | N/A         | N/A              |
|                    |               | or details of the specific API |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/ApiInfo


