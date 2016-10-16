DWDMModuleState Model Objects
============================================

*state/DWDMModule*
------------------------------------

- Multiple objects of this type can exist in a system.

+------------------------+---------------+--------------------------------+-------------+------------------+
|   **PARAMETER NAME**   | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]**     | uint8         | DWDM Module identifier         | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VendorName             | string        | Vendor name of dwdm module     | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleHWVersion        | string        | HW version of dwdm module      | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| Populated              | bool          | Is module populated            | N/A         | N/A              |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VendorDateCode         | string        | Device manufacture data code   | N/A         | N/A              |
|                        |               | of dwdm module                 |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VendorSerialNum        | string        | Vendor assigned serial number  | N/A         | N/A              |
|                        |               | of dwdm module                 |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleActiveFWVersion  | string        | Firmware version of active     | N/A         | N/A              |
|                        |               | partition of dwdm module       |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleState            | string        | Current MSA state of dwdm      | N/A         | N/A              |
|                        |               | module                         |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleStandByFWVersion | string        | Firmware version of standby    | N/A         | N/A              |
|                        |               | partition of dwdm module       |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleVoltage          | float64       | Module power supply voltage in | N/A         | N/A              |
|                        |               | Volts                          |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleStandByFWStatus  | string        | Firmware image status of       | N/A         | N/A              |
|                        |               | standby partition of dwdm      |             |                  |
|                        |               | module                         |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleTemp             | float64       | Module temperature in deg      | N/A         | N/A              |
|                        |               | Celsius                        |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| VendorPartNum          | string        | Vendor assigned part number of | N/A         | N/A              |
|                        |               | dwdm module                    |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+
| ModuleActiveFWStatus   | string        | Firmware image status of       | N/A         | N/A              |
|                        |               | active partition of dwdm       |             |                  |
|                        |               | module                         |             |                  |
+------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModule
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModule?CurrentMarker=<x>&Count=<y>


