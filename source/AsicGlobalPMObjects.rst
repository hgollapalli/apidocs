AsicGlobalPM Model Objects
============================================

*config/AsicGlobalPM*
------------------------------------

- Only one of these object can exist in a system.
- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- **Possible Values**: Temperature
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: Module identifier.
	- This parameter is key element.
- **HighAlarmThreshold**
	- **Data Type**: float64
	- **Description**: High alarm threshold value for this PM.
	- **Default**: 100000
- **HighWarnThreshold**
	- **Data Type**: float64
	- **Description**: High warning threshold value for this PM.
	- **Default**: 100000
- **PMClassBEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-B PM.
	- **Default**: true
- **PMClassCEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-C PM.
	- **Default**: true
- **LowAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Low alarm threshold value for this PM.
	- **Default**: -100000
- **LowWarnThreshold**
	- **Data Type**: float64
	- **Description**: Low warning threshold value for this PM.
	- **Default**: -100000
- **PMClassAEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-A PM.
	- **Default**: true


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/AsicGlobalPM
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/AsicGlobalPM/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/AsicGlobalPM
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/AsicGlobalPM<uuid>


