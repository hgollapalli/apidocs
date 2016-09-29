QsfpChannelPMDataState Model Objects
============================================

*state/QsfpChannelPMData*
------------------------------------

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


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/QsfpChannelPMData


