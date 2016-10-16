EthernetPM Model Objects
============================================

*config/EthernetPM*
------------------------------------

- Multiple of these objects can exist in a system.
- **IntfRef**
	- **Data Type**: string
	- **Description**: Interface name of port.
	- This parameter is key element.
- **Resource**
	- **Data Type**: string
	- **Description**: Resource identifier.
	- **Possible Values**: StatUnderSizePkts, StatOverSizePkts, StatFragments, StatCRCAlignErrors, StatJabber, StatEtherPkts, StatMCPkts, StatBCPkts, Stat64OctOrLess, Stat65OctTo126Oct, Stat128OctTo255Oct, Stat128OctTo255Oct, Stat256OctTo511Oct, Stat512OctTo1023Oct, Statc1024OctTo1518Oct
	- This parameter is key element.
- **PMClassBEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-B PM.
	- **Default**: true
- **PMClassCEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-C PM.
	- **Default**: true
- **HighAlarmThreshold**
	- **Data Type**: float64
	- **Description**: High alarm threshold value for this PM.
	- **Default**: 100000
- **LowAlarmThreshold**
	- **Data Type**: float64
	- **Description**: Low alarm threshold value for this PM.
	- **Default**: -100000
- **PMClassAEnable**
	- **Data Type**: bool
	- **Description**: Enable/Disable control for CLASS-A PM.
	- **Default**: true
- **HighWarnThreshold**
	- **Data Type**: float64
	- **Description**: High warning threshold value for this PM.
	- **Default**: 100000
- **LowWarnThreshold**
	- **Data Type**: float64
	- **Description**: Low warning threshold value for this PM.
	- **Default**: -100000


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/EthernetPM
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/EthernetPM/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/EthernetPM?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/EthernetPM
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/EthernetPM<uuid>

