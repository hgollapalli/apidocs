DWDMModuleNwIntfState Model Objects
============================================

*state/DWDMModuleNwIntf*
------------------------------------

- Multiple of these objects can exist in a system.
- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **NwIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module network interface identifier.
	- This parameter is key element.
- **MaxChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **MinChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **MinBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Minimum value of BER over the last PM interval for the DWDM module network interface.
- **RxPower**
	- **Data Type**: float64
	- **Description**: Current RX power for the DWDM module network interface.
- **AvgBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Average value of BER over the last PM interval for the DWDM module network interface.
- **AvgChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Average RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **CurrUncorrectableFECBlkCnt**
	- **Data Type**: float64
	- **Description**: Current value of uncorrectable FEC code block count.
- **CurrentBER**
	- **Data Type**: float64
	- **Description**: Current value of BER on the DWDM module network interface.
- **UncorrectableFECBlkCntOverPMInt**
	- **Data Type**: float64
	- **Description**: Average value of uncorrectable FEC code block count over the last PM interval.
- **CurrChromDisp**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion for the DWDM module network interface.
- **MaxBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Maximum value of BER over the last PM interval for the DWDM module network interface.
- **PRBSRxErrCnt**
	- **Data Type**: float64
	- **Description**: RX PRBS error count for network interface.
- **TxChanGridSpacing**
	- **Data Type**: string
	- **Description**: The channel grid spacing used for this network interface in GHz.
- **ChanFrequency**
	- **Data Type**: float64
	- **Description**: Channel frequency corresponding to selected channel number for the DWDM module network interface.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntf
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModuleNwIntf?CurrentMarker=<x>&Count=<y>


