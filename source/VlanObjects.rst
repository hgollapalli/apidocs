Vlan Model Objects
============================================

*config/Vlan*
------------------------------------

- Multiple of these objects can exist in a system.
- **VlanId**
	- **Data Type**: int32
	- **Description**: 802.1Q tag/Vlan ID for vlan being provisioned.
	- This parameter is key element.
- **IntfList**
	- **Data Type**: string
	- **Description**: List of interface names or ifindex values to  be added as tagged members of the vlan.
- **UntagIntfList**
	- **Data Type**: string
	- **Description**: List of interface names or ifindex values to  be added as untagged members of the vlan.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Vlan
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/Vlan?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Vlan<uuid>


