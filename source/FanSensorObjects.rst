FanSensor Model Objects
============================================

*config/FanSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+------------------------+---------------+--------------------------------+-------------+------------------+
|   **PARAMETER NAME**   | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+------------------------+---------------+--------------------------------+-------------+------------------+
| Name **[KEY]**         | string        | Fan Sensor Name                | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmThreshold    | int32         | Lower Alarm Threshold for TCA  | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState     | string        | PM Class-A Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmThreshold   | int32         | Higher Alarm Threshold for TCA | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningThreshold | int32         | Higher Warning Threshold for   | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState     | string        | PM Class-B Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState     | string        | PM Class-C Admin State         | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| AdminState             | string        | Enable/Disable                 | Enable      | Enable, Disable  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningThreshold  | int32         | Lower Warning Threshold for    | N/A         | N/A              |
|                        |               | TCA                            |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FanSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor<uuid>


