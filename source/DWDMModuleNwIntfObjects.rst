DWDMModuleNwIntf Model Objects
============================================

*config/DWDMModuleNwIntf*
------------------------------------

- **NwIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module network interface identifier.
	- This parameter is key element.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **TxPRBSInvertPattern**
	- **Data Type**: bool
	- **Description**: Generate inverted PRBS polynomial pattern.
	- **Default**: true
- **TxPRBSPattern**
	- **Data Type**: string
	- **Description**: Pattern to use for TX PRBS generation.
	- **Default**: 2^31
- **TxPulseShapeFltrRollOff**
	- **Data Type**: float64
	- **Description**: TX pulse shape filter roll off factor.
	- **Default**: 0.301
- **ClntIntfIdToTributary0Map**
	- **Data Type**: uint8
	- **Description**: Client interface ID to map to network interface tributary 0.
- **RxPRBSInvertPattern**
	- **Data Type**: bool
	- **Description**: Check against inverted PRBS polynomial pattern.
	- **Default**: true
- **RxPRBSPattern**
	- **Data Type**: string
	- **Description**: PRBS pattern to use for checker.
	- **Default**: 2^31
- **TxPulseShapeFltrType**
	- **Data Type**: string
	- **Description**: TX pulse shaping filter type.
	- **Default**: RootRaisedCos
- **EnableTxPRBS**
	- **Data Type**: bool
	- **Description**: Enable TX PRBS generation on this network interface.
	- **Default**: false
- **FECMode**
	- **Data Type**: string
	- **Description**: DWDM Module network interface FEC mode.
	- **Default**: 15%SDFEC
- **ModulationFmt**
	- **Data Type**: string
	- **Description**: Modulation format to use for this network interface.
	- **Default**: 16QAM
- **ChannelNumber**
	- **Data Type**: uint8
	- **Description**: TX Channel number to use for this network interface.
	- **Default**: 48
- **ClntIntfIdToTributary1Map**
	- **Data Type**: uint8
	- **Description**: Client interface ID to map to network interface tributary 1.
- **TxPowerRampdBmPerSec**
	- **Data Type**: float64
	- **Description**: Rate of change of tx power on this network interface.
	- **Default**: 1
- **AdminState**
	- **Data Type**: string
	- **Description**: Administrative state of this network interface.
	- **Default**: UP
- **DiffEncoding**
	- **Data Type**: bool
	- **Description**: Control to enable/disable DWDM Module network interface encoding type.
	- **Default**: true
- **EnableRxPRBSChecker**
	- **Data Type**: bool
	- **Description**: Enable RX PRBS checker.
	- **Default**: false
- **TxPower**
	- **Data Type**: float64
	- **Description**: Transmit output power for this network interface in dBm.
	- **Default**: 0


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/DWDMModuleNwIntf
	- POST
		 curl -X POST -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/config/DWDMModuleNwIntf
	- DELETE
		 curl -X DELETE -i -H 'Accept:application/json' -d '{<Model Object as json data>}' http://device-management-IP:8080/public/v1//config/DWDMModuleNwIntf
	- PATCH
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://<device-management-IP:8080/public/v1/config/DWDMModuleNwIntf


