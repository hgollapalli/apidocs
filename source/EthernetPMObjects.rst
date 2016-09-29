EthernetPM Model Objects
============================================

*config/EthernetPM*
------------------------------------

- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- **Possible Values**: StatUnderSizePkts, StatOverSizePkts, StatFragments, StatCRCAlignErrors, StatJabber, StatEtherPkts, StatMCPkts, StatBCPkts, Stat64OctOrLess, Stat65OctTo126Oct, Stat128OctTo255Oct, Stat128OctTo255Oct, Stat256OctTo511Oct, Stat512OctTo1023Oct, Statc1024OctTo1518Oct
	- This parameter is key element.
- **IntfRef**
	- **Data Type**: string
	- **Description**: Interface name of port.
	- This parameter is key element.
- **HighAlarmThreshold**
	- **Data Type**: float64
	- **Description**: High alarm threshold value for this PM.
	- **Default**: 100000
- **LowWarnThreshold**
	- **Data Type**: float64
	- **Description**: Low warning threshold value for this PM.
	- **Default**: -100000
- **PMClassAEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-A PM.
	- **Default**: true
- **PMClassBEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-B PM.
	- **Default**: true
- **PMClassCEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-C PM.
	- **Default**: true
- **HighWarnThreshold**
	- **Data Type**: float64
	- **Description**: High warning threshold value for this PM.
	- **Default**: 100000
- **LowAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Low alarm threshold value for this PM.
	- **Default**: -100000


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/EthernetPM
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/EthernetPM
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/EthernetPM
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/EthernetPM


