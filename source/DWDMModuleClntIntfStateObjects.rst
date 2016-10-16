DWDMModuleClntIntfState Model Objects
============================================

*state/DWDMModuleClntIntf*
------------------------------------

- Multiple objects of this type can exist in a system.

+----------------------+---------------+--------------------------------+-------------+------------------+
|  **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+----------------------+---------------+--------------------------------+-------------+------------------+
| ModuleId **[KEY]**   | uint8         | DWDM Module identifier         | N/A         | N/A              |
+----------------------+---------------+--------------------------------+-------------+------------------+
| ClntIntfId **[KEY]** | uint8         | DWDM Module client interface   | N/A         | N/A              |
|                      |               | identifier                     |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PRBSTxErrCntLane0    | float64       | Client interface host lane 0   | N/A         | N/A              |
|                      |               | PRBS TX Error count            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PRBSTxErrCntLane1    | float64       | Client interface host lane 1   | N/A         | N/A              |
|                      |               | PRBS TX Error count            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PRBSTxErrCntLane2    | float64       | Client interface host lane 2   | N/A         | N/A              |
|                      |               | PRBS TX Error count            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+
| PRBSTxErrCntLane3    | float64       | Client interface host lane 3   | N/A         | N/A              |
|                      |               | PRBS TX Error count            |             |                  |
+----------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/DWDMModuleClntIntf
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/DWDMModuleClntIntf?CurrentMarker=<x>&Count=<y>


