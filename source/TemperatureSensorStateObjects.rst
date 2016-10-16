TemperatureSensorState Model Objects
============================================

*state/TemperatureSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+---------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |      **DESCRIPTION**      | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+---------------------------+-------------+------------------+
| Name **[KEY]**     | string        | Temperature Sensor Name   | N/A         | N/A              |
+--------------------+---------------+---------------------------+-------------+------------------+
| CurrentTemperature | float64       | Current Temperature Value | N/A         | N/A              |
+--------------------+---------------+---------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/TemperatureSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/TemperatureSensor?CurrentMarker=<x>&Count=<y>


