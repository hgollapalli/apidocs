PortState Model Objects
============================================

*state/Port*
------------------------------------

- Only one object of this type can exist in a system.

+-----------------------------+---------------+--------------------------------+-------------+------------------+
|     **PARAMETER NAME**      | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** | **VALID VALUES** |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IntfRef **[KEY]**           | string        | Front panel port name or       | N/A         | N/A              |
|                             |               | system assigned interface id   |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| ConfigMode                  | string        | The current mode of            | N/A         | N/A              |
|                             |               | configuration on this port     |             |                  |
|                             |               | (L2/L3/Internal)               |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts1024To1518Octets | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets sized between |             |                  |
|                             |               | 1024 and 1518 bytes            |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts128To255Octets   | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets sized between |             |                  |
|                             |               | 128 and 255 bytes              |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherUnderSizePktCnt      | int64         | RFC 1757 Total numbe of        | N/A         | N/A              |
|                             |               | undersized packets received    |             |                  |
|                             |               | and transmitted                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| Name                        | string        | System assigned vlan name      | N/A         | N/A              |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| NumDownEvents               | int32         | Number of times the            | N/A         | N/A              |
|                             |               | operational state transitioned |             |                  |
|                             |               | from UP to DOWN                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherOverSizePktCnt       | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | oversized packets received and |             |                  |
|                             |               | transmitted                    |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts65To127Octets    | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets sized between |             |                  |
|                             |               | 65 and 127 bytes               |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfOutOctets                 | int64         | RFC2233 Total number of octets | N/A         | N/A              |
|                             |               | transmitted on this port       |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| LastDownEventTime           | string        | Timestamp corresponding to the | N/A         | N/A              |
|                             |               | last UP to DOWN operational    |             |                  |
|                             |               | state change event             |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| LastUpEventTime             | string        | Timestamp corresponding to the | N/A         | N/A              |
|                             |               | last DOWN to UP operational    |             |                  |
|                             |               | state change event             |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherBcastPkts            | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet broadcast packets     |             |                  |
|                             |               | received and transmitted       |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfInOctets                  | int64         | RFC2233 Total number of octets | N/A         | N/A              |
|                             |               | received on this port          |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfInUnknownProtos           | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | inbound packets discarded due  |             |                  |
|                             |               | to unknown protocol            |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfOutUcastPkts              | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | unicast packets transmitted on |             |                  |
|                             |               | this port                      |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| PRBSRxErrCnt                | int64         | Receive error count reported   | N/A         | N/A              |
|                             |               | by PRBS checker                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherCRCAlignError        | int64         | RFC 1757 Total number of CRC   | N/A         | N/A              |
|                             |               | alignment errors               |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts                 | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets received and  |             |                  |
|                             |               | transmitted                    |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts64OrLessOctets   | int64         | RFC1757 Total number of        | N/A         | N/A              |
|                             |               | ethernet packets sized 64      |             |                  |
|                             |               | bytes or lesser                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfInErrors                  | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | inbound packets that contained |             |                  |
|                             |               | an error                       |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfInUcastPkts               | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | unicast packets received on    |             |                  |
|                             |               | this port                      |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| OperState                   | string        | Operational state of front     | N/A         | N/A              |
|                             |               | panel port                     |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| PresentInHW                 | string        | Indication of whether this     | N/A         | N/A              |
|                             |               | port object maps to a physical |             |                  |
|                             |               | port. Set to 'No' for ports    |             |                  |
|                             |               | that are not broken out.       |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts512To1023Octets  | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets sized between |             |                  |
|                             |               | 512 and 1023 bytes             |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherMCPkts               | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | multicast packets received and |             |                  |
|                             |               | transmitted                    |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherFragments            | int64         | RFC1757 Total number of        | N/A         | N/A              |
|                             |               | ethernet fragments received    |             |                  |
|                             |               | and transmitted                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherPkts256To511Octets   | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | ethernet packets sized between |             |                  |
|                             |               | 256 and 511 bytes              |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfInDiscards                | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | inbound packets that were      |             |                  |
|                             |               | discarded                      |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| NumUpEvents                 | int32         | Number of times the            | N/A         | N/A              |
|                             |               | operational state transitioned |             |                  |
|                             |               | from DOWN to UP                |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| Pvid                        | int32         | The vlanid assigned to         | N/A         | N/A              |
|                             |               | untagged traffic ingressing    |             |                  |
|                             |               | this port                      |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| ErrDisableReason            | string        | Reason explaining why port has | N/A         | N/A              |
|                             |               | been disabled by protocol code |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfEtherJabber               | int64         | RFC 1757 Total number of       | N/A         | N/A              |
|                             |               | jabber frames received and     |             |                  |
|                             |               | transmitted                    |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfIndex                     | int32         | System assigned interface id   | N/A         | N/A              |
|                             |               | for this port                  |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfOutDiscards               | int64         | RFC2233 Total number of error  | N/A         | N/A              |
|                             |               | free packets discarded and not |             |                  |
|                             |               | transmitted                    |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+
| IfOutErrors                 | int64         | RFC2233 Total number of        | N/A         | N/A              |
|                             |               | packets discarded and not      |             |                  |
|                             |               | transmitted due to packet      |             |                  |
|                             |               | errors                         |             |                  |
+-----------------------------+---------------+--------------------------------+-------------+------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/Port


