QsfpChannel Model Objects
============================================

*config/QsfpChannel*
------------------------------------

- Multiple of these objects can exist in a system.
- **ChannelNum**
	- **Data Type**: int32
	- **Description**: Qsfp Channel Number.
	- This parameter is key element.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: Qsfp Id.
	- This parameter is key element.
- **HigherWarningTXPower**
	- **Data Type**: float64
	- **Description**: Higher Warning Rx power for TCA.
- **LowerAlarmTXBias**
	- **Data Type**: float64
	- **Description**: Lower Alarm Tx Current Bias for TCA.
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Disable
- **HigherAlarmTXBias**
	- **Data Type**: float64
	- **Description**: Higher Alarm Tx Current Bias for TCA.
- **LowerWarningTXPower**
	- **Data Type**: float64
	- **Description**: Lower Warning Rx power for TCA.
- **HigherAlarmTXPower**
	- **Data Type**: float64
	- **Description**: Higher Alarm Rx power for TCA.
- **HigherWarningRXPower**
	- **Data Type**: float64
	- **Description**: Higher Warning Rx power Threshold for TCA.
- **LowerAlarmRXPower**
	- **Data Type**: float64
	- **Description**: Lower Alarm Rx power Threshold for TCA.
- **LowerAlarmTXPower**
	- **Data Type**: float64
	- **Description**: Lower Alarm Rx power for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Disable
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Disable
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Disable
- **HigherAlarmRXPower**
	- **Data Type**: float64
	- **Description**: Higher Alarm Rx power Threshold for TCA.
- **LowerWarningRXPower**
	- **Data Type**: float64
	- **Description**: Lower Warning Rx power Threshold for TCA.
- **LowerWarningTXBias**
	- **Data Type**: float64
	- **Description**: Lower Warning Tx Current Bias for TCA.
- **HigherWarningTXBias**
	- **Data Type**: float64
	- **Description**: Higher Warning Tx Current Bias for TCA.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/QsfpChannel
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/QsfpChannel?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/QsfpChannel<uuid>


