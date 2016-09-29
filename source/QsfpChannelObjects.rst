QsfpChannel Model Objects
============================================

*config/QsfpChannel*
------------------------------------

- **ChannelNum**
	- **Data Type**: int32
	- **Description**: Qsfp Channel Number.
	- This parameter is key element.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: Qsfp Id.
	- This parameter is key element.
- **LowerWarningTXPower**
	- **Data Type**: float64
	- **Description**: Lower Warning Rx power for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Disable
- **HigherWarningTXBias**
	- **Data Type**: float64
	- **Description**: Higher Warning Tx Current Bias for TCA.
- **LowerAlarmTXBias**
	- **Data Type**: float64
	- **Description**: Lower Alarm Tx Current Bias for TCA.
- **LowerWarningRXPower**
	- **Data Type**: float64
	- **Description**: Lower Warning Rx power Threshold for TCA.
- **HigherWarningTXPower**
	- **Data Type**: float64
	- **Description**: Higher Warning Rx power for TCA.
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Disable
- **HigherAlarmTXPower**
	- **Data Type**: float64
	- **Description**: Higher Alarm Rx power for TCA.
- **HigherWarningRXPower**
	- **Data Type**: float64
	- **Description**: Higher Warning Rx power Threshold for TCA.
- **HigherAlarmTXBias**
	- **Data Type**: float64
	- **Description**: Higher Alarm Tx Current Bias for TCA.
- **LowerAlarmTXPower**
	- **Data Type**: float64
	- **Description**: Lower Alarm Rx power for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Disable
- **LowerWarningTXBias**
	- **Data Type**: float64
	- **Description**: Lower Warning Tx Current Bias for TCA.
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Disable
- **HigherAlarmRXPower**
	- **Data Type**: float64
	- **Description**: Higher Alarm Rx power Threshold for TCA.
- **LowerAlarmRXPower**
	- **Data Type**: float64
	- **Description**: Lower Alarm Rx power Threshold for TCA.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/QsfpChannel
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/QsfpChannel
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/QsfpChannel
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/QsfpChannel


