SystemSwVersionState Model Objects
============================================

*state/SystemSwVersion*
------------------------------------

- **FlexswitchVersion**
	- **Data Type**: string
	- **Description**: Flexswitch version.
	- This parameter is key element.
- **Repos**
	- **Data Type**: RepoInfo
	- **Description**: Git repo details.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/SystemSwVersion


