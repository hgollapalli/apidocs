PowerConverterSensorState Model Objects
============================================

*state/PowerConverterSensor*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+-----------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |       **DESCRIPTION**       | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+-----------------------------+-------------+------------------+
| Name **[KEY]**     | string        | Power Converter Sensor Name | N/A         | N/A              |
+--------------------+---------------+-----------------------------+-------------+------------------+
| CurrentPower       | float64       | Current Output Power Value  | N/A         | N/A              |
+--------------------+---------------+-----------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PowerConverterSensor
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/PowerConverterSensor?CurrentMarker=<x>&Count=<y>


