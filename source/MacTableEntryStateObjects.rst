MacTableEntryState Model Objects
============================================

*state/MacTableEntry*
------------------------------------

- **MacAddr**
	- **Data Type**: string
	- **Description**: MAC Address.
	- This parameter is key element.
- **Port**
	- **Data Type**: int32
	- **Description**: Port number on which mac was learned.
	- **Default**: 0
- **VlanId**
	- **Data Type**: int32
	- **Description**: Vlan id corresponding to which mac was learned.
	- **Default**: 0


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/MacTableEntry


