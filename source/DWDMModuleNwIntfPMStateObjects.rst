DWDMModuleNwIntfPMState Model Objects
============================================

*state/DWDMModuleNwIntfPM*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+------------------+--------------------------------+-------------+---------------------------+
| **PARAMETER NAME** |  **DATA TYPE**   |        **DESCRIPTION**         | **DEFAULT** |     **VALID VALUES**      |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| Class **[KEY]**    | string           | Class of PM Data               | CLASS-A     | CLASS-A, CLASS-B, CLASS-B |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| ModuleId **[KEY]** | uint8            | DWDM Module identifier         | N/A         | N/A                       |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| NwIntfId **[KEY]** | uint8            | DWDM Module network interface  | N/A         | N/A                       |
|                    |                  | identifier                     |             |                           |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| Resource **[KEY]** | string           | Opticd resource name for which | N/A         | N/A                       |
|                    |                  | PM Data is required            |             |                           |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| Type **[KEY]**     | string           | Min/Max/Avg                    | N/A         | N/A                       |
+--------------------+------------------+--------------------------------+-------------+---------------------------+
| Data               | DWDMModulePMData |                                | N/A         | N/A                       |
+--------------------+------------------+--------------------------------+-------------+---------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntfPM
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntfPM?CurrentMarker=<x>&Count=<y>


