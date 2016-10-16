QsfpChannelState Model Objects
============================================

*state/QsfpChannel*
------------------------------------

- Multiple objects of this type can exist in a system.

+----------------------+---------------+------------------------------+-------------+------------------+
|  **PARAMETER NAME**  | **DATA TYPE** |       **DESCRIPTION**        | **DEFAULT** | **VALID VALUES** |
+----------------------+---------------+------------------------------+-------------+------------------+
| ChannelNum **[KEY]** | int32         | Qsfp Channel Number          | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+
| QsfpId **[KEY]**     | int32         | QSFP Id                      | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+
| TXPower              | float64       | Rx power on channel 1        | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+
| Present              | bool          | Present or Not Value         | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+
| RXPower              | float64       | Rx power on channel 1        | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+
| TXBias               | float64       | Tx Current Bias on channel 1 | N/A         | N/A              |
+----------------------+---------------+------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/QsfpChannel
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/QsfpChannel?CurrentMarker=<x>&Count=<y>


