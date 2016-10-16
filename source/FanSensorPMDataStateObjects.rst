FanSensorPMDataState Model Objects
============================================

*state/FanSensorPMData*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+-----------------+------------------+-------------+---------------------------+
| **PARAMETER NAME** |  **DATA TYPE**  | **DESCRIPTION**  | **DEFAULT** |     **VALID VALUES**      |
+--------------------+-----------------+------------------+-------------+---------------------------+
| Name **[KEY]**     | string          | Fan Sensor Name  | N/A         | N/A                       |
+--------------------+-----------------+------------------+-------------+---------------------------+
| Class **[KEY]**    | string          | Class of PM Data | CLASS-A     | CLASS-A, CLASS-B, CLASS-B |
+--------------------+-----------------+------------------+-------------+---------------------------+
| Data               | FanSensorPMData |                  | N/A         | N/A                       |
+--------------------+-----------------+------------------+-------------+---------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/FanSensorPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/FanSensorPMData?CurrentMarker=<x>&Count=<y>


