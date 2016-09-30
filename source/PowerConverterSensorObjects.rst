PowerConverterSensor Model Objects
============================================

*config/PowerConverterSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Power Converter Sensor Name.
	- This parameter is key element.
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Enable
- **HigherAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Higher Alarm Threshold for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Enable
- **LowerAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Lower Alarm Threshold for TCA.
- **LowerWarningThreshold**
	- **Data Type**: float64
	- **Description**: Lower Warning Threshold for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Enable
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Enable
- **HigherWarningThreshold**
	- **Data Type**: float64
	- **Description**: Higher Warning Threshold for TCA.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/PowerConverterSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/PowerConverterSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/PowerConverterSensor?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/PowerConverterSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/PowerConverterSensor<uuid>


