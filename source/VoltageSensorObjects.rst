VoltageSensor Model Objects
============================================

*config/VoltageSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Voltage Sensor Name.
	- This parameter is key element.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Enable
- **HigherWarningThreshold**
	- **Data Type**: float64
	- **Description**: Higher Warning Threshold for TCA.
- **LowerWarningThreshold**
	- **Data Type**: float64
	- **Description**: Lower Warning Threshold for TCA.
- **LowerAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Lower Alarm Threshold for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Enable
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Enable
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Enable
- **HigherAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Higher Alarm Threshold for TCA.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/VoltageSensor
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/VoltageSensor


