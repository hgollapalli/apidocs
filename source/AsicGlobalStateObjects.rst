AsicGlobalState Model Objects
============================================

*state/AsicGlobal*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]** | uint8         | Module identifier              | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ModuleTemp         | float64       | Current module temperature     | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| PartNumber         | string        | Part number of underlying      | N/A         | N/A              |
|                    |               | switching asic                 |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| RevisionId         | string        | Revision ID of underlying      | N/A         | N/A              |
|                    |               | switching asic                 |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| VendorId           | string        | Vendor identification value    | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/AsicGlobal


