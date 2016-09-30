TemperatureSensor Model Objects
============================================

*config/TemperatureSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Temperature Sensor Name.
	- This parameter is key element.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Enable
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Enable
- **HigherAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Higher Alarm Threshold for TCA.
- **HigherWarningThreshold**
	- **Data Type**: float64
	- **Description**: Higher Warning Threshold for TCA.
- **LowerAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Lower Alarm Threshold for TCA.
- **LowerWarningThreshold**
	- **Data Type**: float64
	- **Description**: Lower Warning Threshold for TCA.
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Enable
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Enable


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/TemperatureSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/TemperatureSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/TemperatureSensor?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/TemperatureSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/TemperatureSensor<uuid>


