MacTableEntryState Model Objects
============================================

*state/MacTableEntry*
------------------------------------

- Only one of these object can exist in a system.
- **MacAddr**
	- **Data Type**: string
	- **Description**: MAC Address.
	- This parameter is key element.
- **VlanId**
	- **Data Type**: int32
	- **Description**: Vlan id corresponding to which mac was learned.
	- **Default**: 0
- **Port**
	- **Data Type**: int32
	- **Description**: Port number on which mac was learned.
	- **Default**: 0


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/MacTableEntry


