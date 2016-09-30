FanSensor Model Objects
============================================

*config/FanSensor*
------------------------------------

- Multiple of these objects can exist in a system.
- **Name**
	- **Data Type**: string
	- **Description**: Fan Sensor Name.
	- This parameter is key element.
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Enable
- **LowerAlarmThreshold**
	- **Data Type**: int32
	- **Description**: Lower Alarm Threshold for TCA.
- **LowerWarningThreshold**
	- **Data Type**: int32
	- **Description**: Lower Warning Threshold for TCA.
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Enable
- **HigherAlarmThreshold**
	- **Data Type**: int32
	- **Description**: Higher Alarm Threshold for TCA.
- **HigherWarningThreshold**
	- **Data Type**: int32
	- **Description**: Higher Warning Threshold for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Enable
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Enable


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/FanSensor
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/FanSensor?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/FanSensor<uuid>


