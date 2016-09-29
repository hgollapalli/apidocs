DWDMModuleNwIntfState Model Objects
============================================

*state/DWDMModuleNwIntf*
------------------------------------

- **ModuleId**
	- **Data Type**: uint8
	- **Description**: DWDM Module identifier.
	- This parameter is key element.
- **NwIntfId**
	- **Data Type**: uint8
	- **Description**: DWDM Module network interface identifier.
	- This parameter is key element.
- **ChanFrequency**
	- **Data Type**: float64
	- **Description**: Channel frequency corresponding to selected channel number for the DWDM module network interface.
- **RxPower**
	- **Data Type**: float64
	- **Description**: Current RX power for the DWDM module network interface.
- **UncorrectableFECBlkCntOverPMInt**
	- **Data Type**: float64
	- **Description**: Average value of uncorrectable FEC code block count over the last PM interval.
- **CurrChromDisp**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion for the DWDM module network interface.
- **CurrentBER**
	- **Data Type**: float64
	- **Description**: Current value of BER on the DWDM module network interface.
- **MaxBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Maximum value of BER over the last PM interval for the DWDM module network interface.
- **MaxChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **MinBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Minimum value of BER over the last PM interval for the DWDM module network interface.
- **TxChanGridSpacing**
	- **Data Type**: string
	- **Description**: The channel grid spacing used for this network interface in GHz.
- **AvgBEROverPMInterval**
	- **Data Type**: float64
	- **Description**: Average value of BER over the last PM interval for the DWDM module network interface.
- **AvgChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Average RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **CurrUncorrectableFECBlkCnt**
	- **Data Type**: float64
	- **Description**: Current value of uncorrectable FEC code block count.
- **MinChromDispOverPMInt**
	- **Data Type**: int32
	- **Description**: Current RX chromatic dispersion over the last PM interval for the DWDM module network interface.
- **PRBSRxErrCnt**
	- **Data Type**: float64
	- **Description**: RX PRBS error count for network interface.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/DWDMModuleNwIntf


