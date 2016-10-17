DWDMModuleNwIntf Model Objects
=============================================================

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
| AdminState                | string        | Administrative state of this   | UP            | UP, DOWN                       |
|                           |               | network interface              |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ClntIntfIdToTributary0Map | uint8         | Client interface ID to map to  | N/A           | N/A                            |
|                           |               | network interface tributary 0  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| DiffEncoding              | bool          | Control to enable/disable      | true          | N/A                            |
|                           |               | DWDM Module network interface  |               |                                |
|                           |               | encoding type                  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| FECMode                   | string        | DWDM Module network interface  | 15%SDFEC      | 15%SDFEC, 15%OvrHeadSDFEC,     |
|                           |               | FEC mode                       |               | 25%OvrHeadSDFEC                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPRBSInvertPattern       | bool          | Generate inverted PRBS         | true          | N/A                            |
|                           |               | polynomial pattern             |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPRBSPattern             | string        | Pattern to use for TX PRBS     | 2^31          | 2^7, 2^15, 2^23, 2^31          |
|                           |               | generation                     |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPulseShapeFltrRollOff   | float64       | TX pulse shape filter roll off |         0.301 | N/A                            |
|                           |               | factor                         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ChannelNumber             | uint8         | TX Channel number to use for   |            48 | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPulseShapeFltrType      | string        | TX pulse shaping filter type   | RootRaisedCos | RootRaisedCos, RaisedCos,      |
|                           |               |                                |               | Gaussian                       |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ModulationFmt             | string        | Modulation format to use for   | 16QAM         | QPSK, 8QAM, 16QAM              |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| EnableRxPRBSChecker       | bool          | Enable RX PRBS checker         | false         | N/A                            |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| EnableTxPRBS              | bool          | Enable TX PRBS generation on   | false         | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| RxPRBSInvertPattern       | bool          | Check against inverted PRBS    | true          | N/A                            |
|                           |               | polynomial pattern             |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| RxPRBSPattern             | string        | PRBS pattern to use for        | 2^31          | 2^7, 2^15, 2^23, 2^31          |
|                           |               | checker                        |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPower                   | float64       | Transmit output power for this |             0 | N/A                            |
|                           |               | network interface in dBm       |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| TxPowerRampdBmPerSec      | float64       | Rate of change of tx power on  |             1 | N/A                            |
|                           |               | this network interface         |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+
| ClntIntfIdToTributary1Map | uint8         | Client interface ID to map to  | N/A           | N/A                            |
|                           |               | network interface tributary 1  |               |                                |
+---------------------------+---------------+--------------------------------+---------------+--------------------------------+



*FlexSwitch CURL API Supported*
------------------------------------

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


*FlexSwitch SDK API Supported:*
------------------------------------



- **GET**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getDWDMModuleNwIntf(ModuleId=moduleid, NwIntfId=nwintfid)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **GET By ID**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getDWDMModuleNwIntfById(ObjectId=objectid)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'




- **GET ALL**


::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.getAllDWDMModuleNwIntfs()

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'




- **UPDATE**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.updateDWDMModuleNwIntf(ModuleId=moduleid, NwIntfId=nwintfid, AdminState=adminstate, ClntIntfIdToTributary0Map=clntintfidtotributary0map, DiffEncoding=diffencoding, FECMode=fecmode, TxPRBSInvertPattern=txprbsinvertpattern, TxPRBSPattern=txprbspattern, TxPulseShapeFltrRollOff=txpulseshapefltrrolloff, ChannelNumber=channelnumber, TxPulseShapeFltrType=txpulseshapefltrtype, ModulationFmt=modulationfmt, EnableRxPRBSChecker=enablerxprbschecker, EnableTxPRBS=enabletxprbs, RxPRBSInvertPattern=rxprbsinvertpattern, RxPRBSPattern=rxprbspattern, TxPower=txpower, TxPowerRampdBmPerSec=txpowerrampdbmpersec, ClntIntfIdToTributary1Map=clntintfidtotributary1map)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'


- **UPDATE By ID**

::

	import sys
	import os
	from flexswitchV2 import FlexSwitch

	if __name__ == '__main__':
		switchIP := "192.168.56.101"
		swtch = FlexSwitch (switchIP, 8080)  # Instantiate object to talk to flexSwitch
		response, error = swtch.updateDWDMModuleNwIntfById(ObjectId=objectidAdminState=adminstate, ClntIntfIdToTributary0Map=clntintfidtotributary0map, DiffEncoding=diffencoding, FECMode=fecmode, TxPRBSInvertPattern=txprbsinvertpattern, TxPRBSPattern=txprbspattern, TxPulseShapeFltrRollOff=txpulseshapefltrrolloff, ChannelNumber=channelnumber, TxPulseShapeFltrType=txpulseshapefltrtype, ModulationFmt=modulationfmt, EnableRxPRBSChecker=enablerxprbschecker, EnableTxPRBS=enabletxprbs, RxPRBSInvertPattern=rxprbsinvertpattern, RxPRBSPattern=rxprbspattern, TxPower=txpower, TxPowerRampdBmPerSec=txpowerrampdbmpersec, ClntIntfIdToTributary1Map=clntintfidtotributary1map)

		if error != None: #Error not being None implies there is some problem
			print error
		else :
			print 'Success'
