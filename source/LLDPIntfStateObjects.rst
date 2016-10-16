LLDPIntfState Model Objects
============================================

*state/LLDPIntf*
------------------------------------

- Multiple objects of this type can exist in a system.

+---------------------+---------------+--------------------------------+-------------+------------------+
| **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+---------------------+---------------+--------------------------------+-------------+------------------+
| IntfRef **[KEY]**   | string        | IntfRef where lldp is          | N/A         | N/A              |
|                     |               | configured                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| HoldTime            | string        | Validity of the peer           | N/A         | N/A              |
|                     |               | information                    |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| LocalPort           | string        | Local interface                | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerHostName        | string        | Name of the peer host          | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerMac             | string        | Mac address of direct          | N/A         | N/A              |
|                     |               | connection                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| PeerPort            | string        | Name of directtly connected    | N/A         | N/A              |
|                     |               | pors                           |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| ReceivedFrames      | int32         | Total Frames received from     | N/A         | N/A              |
|                     |               | neighbor                       |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SendFrames          | int32         | Total Frames send to the       | N/A         | N/A              |
|                     |               | neighbor                       |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SystemCapabilities  | string        | System Capabilities of the     | N/A         | N/A              |
|                     |               | peer port                      |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| SystemDescription   | string        | System Description of the peer | N/A         | N/A              |
|                     |               | port                           |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| Enable              | bool          | Enable/Disable lldp config     | N/A         | N/A              |
+---------------------+---------------+--------------------------------+-------------+------------------+
| EnabledCapabilities | string        | Enabled Capabilities of the    | N/A         | N/A              |
|                     |               | peer port                      |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+
| IfIndex             | int32         | IfIndex where lldp needs to be | N/A         | N/A              |
|                     |               | configured                     |             |                  |
+---------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/LLDPIntf
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/state/LLDPIntf?CurrentMarker=<x>&Count=<y>


