VlanState Model Objects
============================================

*state/Vlan*
------------------------------------

- Multiple of these objects can exist in a system.
- **VlanId**
	- **Data Type**: int32
	- **Description**: 802.1Q tag/Vlan ID for vlan being provisioned.
	- This parameter is key element.
- **VlanName**
	- **Data Type**: string
	- **Description**: System assigned vlan name.
- **IfIndex**
	- **Data Type**: int32
	- **Description**: System assigned interface id for this vlan interface.
- **OperState**
	- **Data Type**: string
	- **Description**: Operational state of vlan interface.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Vlan
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/Vlan?CurrentMarker=<x>&Count=<y>


