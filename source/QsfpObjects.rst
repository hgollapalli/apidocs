Qsfp Model Objects
============================================

*config/Qsfp*
------------------------------------

- Multiple of these objects can exist in a system.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: Qsfp Id.
	- This parameter is key element.
- **LowerWarningTemperature**
	- **Data Type**: float64
	- **Description**: Lower Warning temperature threshold for TCA.
- **LowerWarningVoltage**
	- **Data Type**: float64
	- **Description**: Lower Warning Voltage threshold for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Disable
- **HigherAlarmVoltage**
	- **Data Type**: float64
	- **Description**: Higher Alarm Voltage threshold for TCA.
- **HigherWarningTemperature**
	- **Data Type**: float64
	- **Description**: Higher Warning temperature threshold for TCA.
- **LowerAlarmTemperature**
	- **Data Type**: float64
	- **Description**: Lower Alarm temperature threshold for TCA.
- **LowerAlarmVoltage**
	- **Data Type**: float64
	- **Description**: Lower Alarm Voltage threshold for TCA.
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Disable
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Disable
- **HigherAlarmTemperature**
	- **Data Type**: float64
	- **Description**: Higher Alarm temperature threshold for TCA.
- **HigherWarningVoltage**
	- **Data Type**: float64
	- **Description**: Higher Warning Voltage threshold for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Disable


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Qsfp
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Qsfp/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/Qsfp?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Qsfp
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Qsfp<uuid>


