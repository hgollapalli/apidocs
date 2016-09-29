Qsfp Model Objects
============================================

*config/Qsfp*
------------------------------------

- **QsfpId**
	- **Data Type**: int32
	- **Description**: Qsfp Id.
	- This parameter is key element.
- **HigherWarningTemperature**
	- **Data Type**: float64
	- **Description**: Higher Warning temperature threshold for TCA.
- **LowerAlarmVoltage**
	- **Data Type**: float64
	- **Description**: Lower Alarm Voltage threshold for TCA.
- **LowerWarningTemperature**
	- **Data Type**: float64
	- **Description**: Lower Warning temperature threshold for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Disable
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Disable
- **HigherAlarmVoltage**
	- **Data Type**: float64
	- **Description**: Higher Alarm Voltage threshold for TCA.
- **HigherWarningVoltage**
	- **Data Type**: float64
	- **Description**: Higher Warning Voltage threshold for TCA.
- **LowerAlarmTemperature**
	- **Data Type**: float64
	- **Description**: Lower Alarm temperature threshold for TCA.
- **LowerWarningVoltage**
	- **Data Type**: float64
	- **Description**: Lower Warning Voltage threshold for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Disable
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Disable
- **HigherAlarmTemperature**
	- **Data Type**: float64
	- **Description**: Higher Alarm temperature threshold for TCA.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/Qsfp
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/Qsfp
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/Qsfp
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/Qsfp


