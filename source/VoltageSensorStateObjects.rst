VoltageSensorState Model Objects
============================================

*state/VoltageSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+-----------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |    **DESCRIPTION**    | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+-----------------------+-------------+------------------+
| Name **[KEY]**     | string        | Voltage Sensor Name   | N/A         | N/A              |
+--------------------+---------------+-----------------------+-------------+------------------+
| CurrentVoltage     | float64       | Current Voltage Value | N/A         | N/A              |
+--------------------+---------------+-----------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/VoltageSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/VoltageSensor?CurrentMarker=<x>&Count=<y>


