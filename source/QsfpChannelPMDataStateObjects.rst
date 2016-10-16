QsfpChannelPMDataState Model Objects
============================================

*state/QsfpChannelPMData*
------------------------------------

- Multiple objects of this type can exist in a system.

+----------------------+-------------------+-----------------------+-------------+---------------------------+
|  **PARAMETER NAME**  |   **DATA TYPE**   |    **DESCRIPTION**    | **DEFAULT** |     **VALID VALUES**      |
+----------------------+-------------------+-----------------------+-------------+---------------------------+
| QsfpId **[KEY]**     | int32             | QSFP Id               | N/A         | N/A                       |
+----------------------+-------------------+-----------------------+-------------+---------------------------+
| Resource **[KEY]**   | string            | QSFP PM Resource Name | N/A         | N/A                       |
+----------------------+-------------------+-----------------------+-------------+---------------------------+
| ChannelNum **[KEY]** | int32             | Qsfp Channel Number   | N/A         | N/A                       |
+----------------------+-------------------+-----------------------+-------------+---------------------------+
| Class **[KEY]**      | string            | Class of PM Data      | CLASS-A     | CLASS-A, CLASS-B, CLASS-B |
+----------------------+-------------------+-----------------------+-------------+---------------------------+
| Data                 | QsfpChannelPMData |                       | N/A         | N/A                       |
+----------------------+-------------------+-----------------------+-------------+---------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/QsfpChannelPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/QsfpChannelPMData?CurrentMarker=<x>&Count=<y>


