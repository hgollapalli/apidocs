VlanState Model Objects
============================================

*state/Vlan*
------------------------------------

- **VlanId**
	- **Data Type**: int32
	- **Description**: 802.1Q tag/Vlan ID for vlan being provisioned.
	- This parameter is key element.
- **IfIndex**
	- **Data Type**: int32
	- **Description**: System assigned interface id for this vlan interface.
- **OperState**
	- **Data Type**: string
	- **Description**: Operational state of vlan interface.
- **VlanName**
	- **Data Type**: string
	- **Description**: System assigned vlan name.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/Vlan


