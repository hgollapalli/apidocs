QsfpChannelState Model Objects
============================================

*state/QsfpChannel*
------------------------------------

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


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/QsfpChannel


