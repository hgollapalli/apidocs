PowerConverterSensor Model Objects
============================================

*config/PowerConverterSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+------------------------+---------------+--------------------------------+-------------+------------------+
|   **PARAMETER NAME**   | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+------------------------+---------------+--------------------------------+-------------+------------------+
| Name **[KEY]**         | string        | Power Converter Sensor Name    | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmThreshold   | float64       | Higher Alarm Threshold for TCA | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmThreshold    | float64       | Lower Alarm Threshold for TCA  | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningThreshold  | float64       | Lower Warning Threshold for    | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState     | string        | PM Class-A Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState     | string        | PM Class-C Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| AdminState             | string        | Enable/Disable                 | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningThreshold | float64       | Higher Warning Threshold for   | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState     | string        | PM Class-B Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/PowerConverterSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/PowerConverterSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/PowerConverterSensor?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/PowerConverterSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/PowerConverterSensor<uuid>


