Vlan Model Objects
============================================

*config/Vlan*
------------------------------------

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


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/Vlan
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/Vlan
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/Vlan
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/Vlan


