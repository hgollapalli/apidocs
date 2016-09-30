Port Model Objects
============================================

*config/Port*
------------------------------------

- Only one of these object can exist in a system.
- **IntfRef**
	- **Data Type**: string
	- **Description**: Front panel port name or system assigned interface id.
	- This parameter is key element.
- **AdminState**
	- **Data Type**: string
	- **Description**: Administrative state of this port.
	- **Default**: DOWN
- **BreakOutMode**
	- **Data Type**: string
	- **Description**: Break out mode for the port. Only applicable on ports that support breakout. Valid modes - 1x40.
- **Description**
	- **Data Type**: string
	- **Description**: User provided string description.
	- **Default**: FP Port
- **LoopbackMode**
	- **Data Type**: string
	- **Description**: Desired loopback setting for this port.
	- **Default**: NONE
- **IfIndex**
	- **Data Type**: int32
	- **Description**: System assigned interface id for this port. Read only attribute.
- **MediaType**
	- **Data Type**: string
	- **Description**: Type of media inserted into this port.
- **PhyIntfType**
	- **Data Type**: string
	- **Description**: Type of internal phy interface.
- **Speed**
	- **Data Type**: int32
	- **Description**: Port speed in Mbps.
- **Autoneg**
	- **Data Type**: string
	- **Description**: Autonegotiation setting for this port.
	- **Default**: OFF
- **Duplex**
	- **Data Type**: string
	- **Description**: Duplex setting for this port.
	- **Default**: Full Duplex
- **EnableFEC**
	- **Data Type**: bool
	- **Description**: Enable/Disable 802.3bj FEC on this interface.
	- **Default**: false
- **MacAddr**
	- **Data Type**: string
	- **Description**: Mac address associated with this port.
- **Mtu**
	- **Data Type**: int32
	- **Description**: Maximum transmission unit size for this port.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/Port
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/Port/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Port
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/Port<uuid>


