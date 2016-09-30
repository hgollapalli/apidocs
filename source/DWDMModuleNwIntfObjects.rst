DWDMModuleNwIntf Model Objects
============================================

*config/DWDMModuleNwIntf*
------------------------------------

- Multiple of these objects can exist in a system.
- **NwIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module network interface identifier.
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **AdminState**
	- **Data Type**: string
	- **Description**: Administrative state of this network interface.
	- **Default**: UP
- **FECMode**
	- **Data Type**: string
	- **Description**: DWDM Module network interface FEC mode.
	- **Default**: 15%SDFEC
- **ModulationFmt**
	- **Data Type**: string
	- **Description**: Modulation format to use for this network interface.
	- **Default**: 16QAM
- **RxPRBSInvertPattern**
	- **Data Type**: bool
	- **Description**: Check against inverted PRBS polynomial pattern.
	- **Default**: true
- **TxPulseShapeFltrRollOff**
	- **Data Type**: float64
	- **Description**: TX pulse shape filter roll off factor.
	- **Default**: 0.301
- **TxPulseShapeFltrType**
	- **Data Type**: string
	- **Description**: TX pulse shaping filter type.
	- **Default**: RootRaisedCos
- **ClntIntfIdToTributary0Map**
	- **Data Type**: uint8
	- **Description**: Client interface ID to map to network interface tributary 0.
- **DiffEncoding**
	- **Data Type**: bool
	- **Description**: Control to enable/disable DWDM Module network interface encoding type.
	- **Default**: true
- **EnableTxPRBS**
	- **Data Type**: bool
	- **Description**: Enable TX PRBS generation on this network interface.
	- **Default**: false
- **TxPower**
	- **Data Type**: float64
	- **Description**: Transmit output power for this network interface in dBm.
	- **Default**: 0
- **ChannelNumber**
	- **Data Type**: uint8
	- **Description**: TX Channel number to use for this network interface.
	- **Default**: 48
- **RxPRBSPattern**
	- **Data Type**: string
	- **Description**: PRBS pattern to use for checker.
	- **Default**: 2^31
- **TxPRBSPattern**
	- **Data Type**: string
	- **Description**: Pattern to use for TX PRBS generation.
	- **Default**: 2^31
- **TxPRBSInvertPattern**
	- **Data Type**: bool
	- **Description**: Generate inverted PRBS polynomial pattern.
	- **Default**: true
- **TxPowerRampdBmPerSec**
	- **Data Type**: float64
	- **Description**: Rate of change of tx power on this network interface.
	- **Default**: 1
- **ClntIntfIdToTributary1Map**
	- **Data Type**: uint8
	- **Description**: Client interface ID to map to network interface tributary 1.
- **EnableRxPRBSChecker**
	- **Data Type**: bool
	- **Description**: Enable RX PRBS checker.
	- **Default**: false


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/DWDMModuleNwIntf
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModuleNwIntf/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/DWDMModuleNwIntf?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModuleNwIntf
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/DWDMModuleNwIntf<uuid>


