SystemSwVersionState Model Objects
============================================

*state/SystemSwVersion*
------------------------------------

- Only one object of this type can exist in a system.

+-----------------------------+---------------+--------------------+-------------+------------------+
|     **PARAMETER NAME**      | **DATA TYPE** |  **DESCRIPTION**   | **DEFAULT** | **VALID VALUES** |
+-----------------------------+---------------+--------------------+-------------+------------------+
| FlexswitchVersion **[KEY]** | string        | Flexswitch version | N/A         | N/A              |
+-----------------------------+---------------+--------------------+-------------+------------------+
| Repos                       | RepoInfo      | Git repo details   | N/A         | N/A              |
+-----------------------------+---------------+--------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/SystemSwVersion


