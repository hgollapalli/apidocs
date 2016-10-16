Qsfp Model Objects
============================================

*config/Qsfp*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------------+---------------+--------------------------------+-------------+------------------+
|    **PARAMETER NAME**    | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| QsfpId **[KEY]**         | int32         | Qsfp Id                        | N/A         | N/A              |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| AdminState               | string        | Enable/Disable                 | Disable     | Enable, Disable  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmTemperature   | float64       | Higher Alarm temperature       | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmTemperature    | float64       | Lower Alarm temperature        | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningVoltage      | float64       | Lower Warning Voltage          | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassAAdminState       | string        | PM Class-A Admin State         | Disable     | Enable, Disable  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassBAdminState       | string        | PM Class-B Admin State         | Disable     | Enable, Disable  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| HigherAlarmVoltage       | float64       | Higher Alarm Voltage threshold | N/A         | N/A              |
|                          |               | for TCA                        |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningTemperature | float64       | Higher Warning temperature     | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| HigherWarningVoltage     | float64       | Higher Warning Voltage         | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| LowerAlarmVoltage        | float64       | Lower Alarm Voltage threshold  | N/A         | N/A              |
|                          |               | for TCA                        |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| LowerWarningTemperature  | float64       | Lower Warning temperature      | N/A         | N/A              |
|                          |               | threshold for TCA              |             |                  |
+--------------------------+---------------+--------------------------------+-------------+------------------+
| PMClassCAdminState       | string        | PM Class-C Admin State         | Disable     | Enable, Disable  |
+--------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Qsfp
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Qsfp/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/Qsfp?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Qsfp
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Qsfp<uuid>


