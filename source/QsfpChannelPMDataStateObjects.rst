QsfpChannelPMDataState Model Objects
============================================

*state/QsfpChannelPMData*
------------------------------------

- Multiple of these objects can exist in a system.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: QSFP Id.
	- This parameter is key element.
- **Resource**
	- **Data Type**: string
	- **Description**: QSFP PM Resource Name.
	- This parameter is key element.
- **ChannelNum**
	- **Data Type**: int32
	- **Description**: Qsfp Channel Number.
	- This parameter is key element.
- **Class**
	- **Data Type**: string
	- **Description**: Class of PM Data.
	- **Default**: CLASS-A
	- **Possible Values**: CLASS-A, CLASS-B, CLASS-B
	- This parameter is key element.
- **Data**
	- **Data Type**: QsfpChannelPMData
	- **Description**: .


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/QsfpChannelPMData
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/QsfpChannelPMData?CurrentMarker=<x>&Count=<y>


