XponderGlobal Model Objects
============================================

*config/XponderGlobal*
------------------------------------

- Only one object of this type can exist in a system.

+---------------------+---------------+--------------------------------+----------------------------+--------------------------------+
| **PARAMETER NAME**  | **DATA TYPE** |        **DESCRIPTION**         |        **DEFAULT**         |        **VALID VALUES**        |
+---------------------+---------------+--------------------------------+----------------------------+--------------------------------+
| XponderId **[KEY]** | uint8         | Xponder module identifier      |                          0 | N/A                            |
+---------------------+---------------+--------------------------------+----------------------------+--------------------------------+
| XponderDescription  | string        | User configurable description  | This is a Voyager platform | N/A                            |
|                     |               | string for the xponder module  |                            |                                |
+---------------------+---------------+--------------------------------+----------------------------+--------------------------------+
| XponderMode         | string        | Global operational mode of     | OutOfService               | InServiceWire, InServiceRegen, |
|                     |               | Xponder module                 |                            | InServiceOverSub,              |
|                     |               |                                |                            | InServicePacketOptical,        |
|                     |               |                                |                            | OutOfService                   |
+---------------------+---------------+--------------------------------+----------------------------+--------------------------------+


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/config/XponderGlobal
	- GET By ID
		 curl -X GET http://device-management-IP:8080/public/v1/config/XponderGlobal/<uuid>
	- UPDATE(PATCH) By Key
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/XponderGlobal
	- UPDATE(PATCH) By ID
		 curl -X PATCH -H 'Content-Type: application/json' -d '{<Model Object as json data>}'  http://device-management-IP:8080/public/v1/config/XponderGlobal<uuid>


