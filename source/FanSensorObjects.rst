FanSensor Model Objects
============================================

*config/FanSensor*
------------------------------------

- **Name**
	- **Data Type**: string
	- **Description**: Fan Sensor Name.
	- This parameter is key element.
- **AdminState**
	- **Data Type**: string
	- **Description**: Enable/Disable.
	- **Default**: Enable
- **HigherAlarmThreshold**
	- **Data Type**: int32
	- **Description**: Higher Alarm Threshold for TCA.
- **LowerAlarmThreshold**
	- **Data Type**: int32
	- **Description**: Lower Alarm Threshold for TCA.
- **LowerWarningThreshold**
	- **Data Type**: int32
	- **Description**: Lower Warning Threshold for TCA.
- **PMClassAAdminState**
	- **Data Type**: string
	- **Description**: PM Class-A Admin State.
	- **Default**: Enable
- **PMClassCAdminState**
	- **Data Type**: string
	- **Description**: PM Class-C Admin State.
	- **Default**: Enable
- **HigherWarningThreshold**
	- **Data Type**: int32
	- **Description**: Higher Warning Threshold for TCA.
- **PMClassBAdminState**
	- **Data Type**: string
	- **Description**: PM Class-B Admin State.
	- **Default**: Enable


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/FanSensor
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/FanSensor
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/FanSensor
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/FanSensor


