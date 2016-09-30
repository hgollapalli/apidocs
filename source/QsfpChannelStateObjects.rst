QsfpChannelState Model Objects
============================================

*state/QsfpChannel*
------------------------------------

- Multiple of these objects can exist in a system.
- **ChannelNum**
	- **Data Type**: int32
	- **Description**: Qsfp Channel Number.
	- This parameter is key element.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: QSFP Id.
	- This parameter is key element.
- **Present**
	- **Data Type**: bool
	- **Description**: Present or Not Value.
- **RXPower**
	- **Data Type**: float64
	- **Description**: Rx power on channel 1.
- **TXBias**
	- **Data Type**: float64
	- **Description**: Tx Current Bias on channel 1.
- **TXPower**
	- **Data Type**: float64
	- **Description**: Rx power on channel 1.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/QsfpChannel
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/QsfpChannel?CurrentMarker=<x>&Count=<y>


