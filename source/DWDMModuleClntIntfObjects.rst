DWDMModuleClntIntf Model Objects
============================================

*config/DWDMModuleClntIntf*
------------------------------------

- Multiple of these objects can exist in a system.
- **ClntIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module client interface identifier.
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **RXFECDecDisable**
	- **Data Type**: bool
	- **Description**: 802.3bj FEC decoder enable/disable state for traffic from DWDM module to Host.
	- **Default**: false
- **RxPRBSPattern**
	- **Data Type**: string
	- **Description**: RX PRBS generator pattern.
	- **Default**: 2^31
- **TXFECDecDisable**
	- **Data Type**: bool
	- **Description**: 802.3bj FEC decoder enable/disable state for traffic from Host to DWDM Module.
	- **Default**: false
- **EnableHostLoopback**
	- **Data Type**: bool
	- **Description**: Enable/Disable loopback on all host lanes of this client interface.
	- **Default**: false
- **HostTxEqLfCtle**
	- **Data Type**: uint8
	- **Description**: Host interface TX deserializer equalization. LELPZRC LF-CTLE LFPZ gain code..
	- **Default**: 0
- **NwLaneTributaryToClntIntfMap**
	- **Data Type**: uint8
	- **Description**: Network lane/tributary id to map to client interface.
- **AdminState**
	- **Data Type**: string
	- **Description**: Administrative state of this client interface.
	- **Default**: UP
- **EnableRxPRBS**
	- **Data Type**: bool
	- **Description**: Enable/Disable RX PRBS generation for all lanes of this client interface.
	- **Default**: false
- **HostRxSerializerTap0Gain**
	- **Data Type**: uint8
	- **Description**: Host RX Serializer tap 0 control.
	- **Default**: 7
- **HostRxSerializerTap1Gain**
	- **Data Type**: uint8
	- **Description**: Host RX Serializer tap 1 control.
	- **Default**: 7
- **HostRxSerializerTap2Delay**
	- **Data Type**: uint8
	- **Description**: Host RX Serializer tap 2 control.
	- **Default**: 5
- **HostRxSerializerTap2Gain**
	- **Data Type**: uint8
	- **Description**: Host RX Serializer tap 2 control.
	- **Default**: 15
- **TxPRBSPattern**
	- **Data Type**: string
	- **Description**: PRBS pattern to use for checker.
	- **Default**: 2^31
- **HostTxEqDfe**
	- **Data Type**: uint8
	- **Description**: Host interface TX deserializer equalization. s-DFE.
	- **Default**: 0
- **EnableIntSerdesNWLoopback**
	- **Data Type**: bool
	- **Description**: Enable/Disable serdes internal loopback.
	- **Default**: false
- **EnableTxPRBSChecker**
	- **Data Type**: bool
	- **Description**: Enable/Disable TX PRBS checker for all lanes of this client interface.
	- **Default**: false
- **HostRxSerializerTap0Delay**
	- **Data Type**: uint8
	- **Description**: Host RX Serializer tap 0 control.
	- **Default**: 7
- **HostTxEqCtle**
	- **Data Type**: uint8
	- **Description**: Host interface TX deserializer equalization. LELRC CTLE LE gain code..
	- **Default**: 18


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/DWDMModuleClntIntf
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModuleClntIntf/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModuleClntIntf?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModuleClntIntf
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModuleClntIntf<uuid>


