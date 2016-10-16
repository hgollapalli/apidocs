PlatformMgmtDeviceState Model Objects
============================================

*state/PlatformMgmtDevice*
------------------------------------

- Only one object of this type can exist in a system.

+----------------------+---------------+-----------------------------+-------------+------------------+
|  **PARAMETER NAME**  | **DATA TYPE** |       **DESCRIPTION**       | **DEFAULT** | **VALID VALUES** |
+----------------------+---------------+-----------------------------+-------------+------------------+
| DeviceName **[KEY]** | string        | Device Name                 | BMC         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| Version              | string        | Version                     | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| CPUUsage             | string        | CPU Usage                   | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| Description          | string        | Platform Description        | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| MemoryUsage          | string        | Memory Usage                | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| ResetReason          | string        | Reset Reason                | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+
| Uptime               | string        | Uptime and load description | N/A         | N/A              |
+----------------------+---------------+-----------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/PlatformMgmtDevice


