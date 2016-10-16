PowerConverterSensorPMDataState Model Objects
============================================

*state/PowerConverterSensorPMData*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| **PARAMETER NAME** |       **DATA TYPE**        |       **DESCRIPTION**       | **DEFAULT** |     **VALID VALUES**      |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Class **[KEY]**    | string                     | Class of PM Data            | CLASS-A     | CLASS-A, CLASS-B, CLASS-B |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Name **[KEY]**     | string                     | Power Converter Sensor Name | N/A         | N/A                       |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+
| Data               | PowerConverterSensorPMData |                             | N/A         | N/A                       |
+--------------------+----------------------------+-----------------------------+-------------+---------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/PowerConverterSensorPMData?CurrentMarker=<x>&Count=<y>


