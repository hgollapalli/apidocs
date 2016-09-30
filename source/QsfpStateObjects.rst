QsfpState Model Objects
============================================

*state/Qsfp*
------------------------------------

- Multiple of these objects can exist in a system.
- **QsfpId**
	- **Data Type**: int32
	- **Description**: QSFP Id.
	- This parameter is key element.
- **Present**
	- **Data Type**: bool
	- **Description**: Present or Not Value.
- **Temperature**
	- **Data Type**: float64
	- **Description**: Current temperature.
- **VendorRevision**
	- **Data Type**: string
	- **Description**: Vendor Revision.
- **VendorSerialNumber**
	- **Data Type**: string
	- **Description**: Vendor Serial Number.
- **Voltage**
	- **Data Type**: float64
	- **Description**: Current Voltage.
- **DataCode**
	- **Data Type**: string
	- **Description**: Data Code.
- **VendorName**
	- **Data Type**: string
	- **Description**: Vendor Name.
- **VendorOUI**
	- **Data Type**: string
	- **Description**: Vendor OUI.
- **VendorPartNumber**
	- **Data Type**: string
	- **Description**: Vendor Part Number.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Qsfp
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Qsfp?CurrentMarker=<x>&Count=<y>


