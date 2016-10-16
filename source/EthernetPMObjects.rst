EthernetPM Model Objects
============================================

*config/EthernetPM*
------------------------------------

- Multiple objects of this type can exist in a system.

+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| **PARAMETER NAME** | **DATA TYPE** |        **DESCRIPTION**         | **DEFAULT** |        **VALID VALUES**        |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| Resource **[KEY]** | string        | Resource identifier            | N/A         | StatUnderSizePkts,             |
|                    |               |                                |             | StatOverSizePkts,              |
|                    |               |                                |             | StatFragments,                 |
|                    |               |                                |             | StatCRCAlignErrors,            |
|                    |               |                                |             | StatJabber, StatEtherPkts,     |
|                    |               |                                |             | StatMCPkts, StatBCPkts,        |
|                    |               |                                |             | Stat64OctOrLess,               |
|                    |               |                                |             | Stat65OctTo126Oct,             |
|                    |               |                                |             | Stat128OctTo255Oct,            |
|                    |               |                                |             | Stat128OctTo255Oct,            |
|                    |               |                                |             | Stat256OctTo511Oct,            |
|                    |               |                                |             | Stat512OctTo1023Oct,           |
|                    |               |                                |             | Statc1024OctTo1518Oct          |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| IntfRef **[KEY]**  | string        | Interface name of port         | N/A         | N/A                            |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| HighAlarmThreshold | float64       | High alarm threshold value for |      100000 | N/A                            |
|                    |               | this PM                        |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| LowAlarmThreshold  | float64       | Low alarm threshold value for  |     -100000 | N/A                            |
|                    |               | this PM                        |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| PMClassAEnable     | bool          | Enable/Disable control for     | true        | N/A                            |
|                    |               | CLASS-A PM                     |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| PMClassBEnable     | bool          | Enable/Disable control for     | true        | N/A                            |
|                    |               | CLASS-B PM                     |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| PMClassCEnable     | bool          | Enable/Disable control for     | true        | N/A                            |
|                    |               | CLASS-C PM                     |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| HighWarnThreshold  | float64       | High warning threshold value   |      100000 | N/A                            |
|                    |               | for this PM                    |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+
| LowWarnThreshold   | float64       | Low warning threshold value    |     -100000 | N/A                            |
|                    |               | for this PM                    |             |                                |
+--------------------+---------------+--------------------------------+-------------+--------------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/EthernetPM
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/EthernetPM/<uuid>
	- GET ALL
		 curl -X GET http://device-management-IP:8080/public/v1/config/EthernetPM?CurrentMarker=<x>&Count=<y>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/EthernetPM
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/EthernetPM<uuid>


