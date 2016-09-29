AsicGlobalPM Model Objects
============================================

*config/AsicGlobalPM*
------------------------------------

- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- **Possible Values**: Temperature
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: Module identifier.
	- This parameter is key element.
- **PMClassBEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-B PM.
	- **Default**: true
- **HighAlarmThreshold**
	- **Data Type**: float64
	- **Description**: High alarm threshold value for this PM.
	- **Default**: 100000
- **HighWarnThreshold**
	- **Data Type**: float64
	- **Description**: High warning threshold value for this PM.
	- **Default**: 100000
- **LowWarnThreshold**
	- **Data Type**: float64
	- **Description**: Low warning threshold value for this PM.
	- **Default**: -100000
- **PMClassAEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-A PM.
	- **Default**: true
- **LowAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Low alarm threshold value for this PM.
	- **Default**: -100000
- **PMClassCEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-C PM.
	- **Default**: true


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/AsicGlobalPM
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/AsicGlobalPM
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/AsicGlobalPM
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/AsicGlobalPM


