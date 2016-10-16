DWDMModule Model Objects
============================================

*config/DWDMModule*
------------------------------------

- Multiple objects of this type can exist in a system.

+---------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+---------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]**  | uint8         | DWDM Module identifier         | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PMInterval          | uint8         | Performance monitoring         |           1 | N/A              |
|                     |               | interval                       |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| AdminState          | string        | Reset state of this dwdm       | DOWN        | UP, DOWN         |
|                     |               | module (false (Reset           |             |                  |
|                     |               | deasserted)                    |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| EnableExtPMTickSrc  | bool          | Enable/Disable external        | false       | N/A              |
|                     |               | tick source for performance    |             |                  |
|                     |               | monitoring                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| IndependentLaneMode | bool          | Network lane configuration     | true        | N/A              |
|                     |               | for the DWDM Module.           |             |                  |
|                     |               | true-Independent lanes         |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/DWDMModule
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModule/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModule?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModule
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModule<uuid>


