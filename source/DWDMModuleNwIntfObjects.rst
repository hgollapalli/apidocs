DWDMModuleNwIntf Model Objects
============================================

*config/DWDMModuleNwIntf*
------------------------------------

- Multiple objects of this type can exist in a system.

+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
|    **PARAMETER NAME**     | **DATA TYPE** |        **DESCRIPTION**         |  **DEFAULT**  |        **VALID VALUES**        |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ModuleId **[KEY]**        | uint8         | DWDM Module identifier         | N/A           | N/A                            |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| NwIntfId **[KEY]**        | uint8         | DWDM Module network interface  | N/A           | N/A                            |
|                           |               | identifier                     |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ClntIntfIdToTributary1Map | uint8         | Client interface ID to map to  | N/A           | N/A                            |
|                           |               | network interface tributary 1  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| AdminState                | string        | Administrative state of this   | UP            | UP, DOWN                       |
|                           |               | network interface              |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| FECMode                   | string        | DWDM Module network interface  | 15%SDFEC      | 15%SDFEC, 15%OvrHeadSDFEC,     |
|                           |               | FEC mode                       |               | 25%OvrHeadSDFEC                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPowerRampdBmPerSec      | float64       | Rate of change of tx power on  |             1 | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPRBSPattern             | string        | Pattern to use for TX PRBS     | 2^31          | 2^7, 2^15, 2^23, 2^31          |
|                           |               | generation                     |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPulseShapeFltrRollOff   | float64       | TX pulse shape filter roll off |         0.301 | N/A                            |
|                           |               | factor                         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPulseShapeFltrType      | string        | TX pulse shaping filter type   | RootRaisedCos | RootRaisedCos, RaisedCos,      |
|                           |               |                                |               | Gaussian                       |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ChannelNumber             | uint8         | TX Channel number to use for   |            48 | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| EnableRxPRBSChecker       | bool          | Enable RX PRBS checker         | false         | N/A                            |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| EnableTxPRBS              | bool          | Enable TX PRBS generation on   | false         | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| RxPRBSPattern             | string        | PRBS pattern to use for        | 2^31          | 2^7, 2^15, 2^23, 2^31          |
|                           |               | checker                        |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| RxPRBSInvertPattern       | bool          | Check against inverted PRBS    | true          | N/A                            |
|                           |               | polynomial pattern             |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPRBSInvertPattern       | bool          | Generate inverted PRBS         | true          | N/A                            |
|                           |               | polynomial pattern             |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPower                   | float64       | Transmit output power for this |             0 | N/A                            |
|                           |               | network interface in dBm       |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ClntIntfIdToTributary0Map | uint8         | Client interface ID to map to  | N/A           | N/A                            |
|                           |               | network interface tributary 0  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| DiffEncoding              | bool          | Control to enable/disable      | true          | N/A                            |
|                           |               | DWDM Module network interface  |               |                                |
|                           |               | encoding type                  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ModulationFmt             | string        | Modulation format to use for   | 16QAM         | QPSK, 8QAM, 16QAM              |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+


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


