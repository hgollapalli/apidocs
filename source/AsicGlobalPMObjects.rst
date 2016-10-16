AsicGlobalPM Model Objects
============================================

*config/AsicGlobalPM*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Resource **[KEY]** | string        | Resource identifier            | N/A         | Temperature      |
+--------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]** | uint8         | Module identifier              |           0 | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| LowAlarmThreshold  | float64       | Low alarm threshold value for  |     -100000 | N/A              |
|                    |               | this PM                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| LowWarnThreshold   | float64       | Low warning threshold value    |     -100000 | N/A              |
|                    |               | for this PM                    |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBEnable     | bool          | Enable/Disable control for     | true        | N/A              |
|                    |               | CLASS-B PM                     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCEnable     | bool          | Enable/Disable control for     | true        | N/A              |
|                    |               | CLASS-C PM                     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| HighAlarmThreshold | float64       | High alarm threshold value for |      100000 | N/A              |
|                    |               | this PM                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| HighWarnThreshold  | float64       | High warning threshold value   |      100000 | N/A              |
|                    |               | for this PM                    |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAEnable     | bool          | Enable/Disable control for     | true        | N/A              |
|                    |               | CLASS-A PM                     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/AsicGlobalPM
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/AsicGlobalPM/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/AsicGlobalPM
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/AsicGlobalPM<uuid>


