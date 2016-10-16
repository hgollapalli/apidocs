LLDPGlobalState Model Objects
============================================

*state/LLDPGlobal*
------------------------------------

- Only one object of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Vrf **[KEY]**      | string        | Vrf where LLDP Global Config   | N/A         | N/A              |
|                    |               | is running                     |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Enable             | bool          | Enable/Disable LLDP Globally   | N/A         | N/A              |
+--------------------+---------------+--------------------------------+-------------+------------------+
| Neighbors          | int32         | Total lldp Neighbors learned   | N/A         | N/A              |
|                    |               | on the system                  |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| TotalRxFrames      | int32         | Total no.of lldp frames        | N/A         | N/A              |
|                    |               | received by the system         |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| TotalTxFrames      | int32         | Total no.of lldp frames send   | N/A         | N/A              |
|                    |               | out by the system              |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+
| TranmitInterval    | int32         | LLDP Re-Transmit Interval in   | N/A         | N/A              |
|                    |               | seconds                        |             |                  |
+--------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/LLDPGlobal


