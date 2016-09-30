ApiInfoState Model Objects
============================================

*state/ApiInfo*
------------------------------------

- Only one of these object can exist in a system.
- **Url**
	- **Data Type**: string
	- **Description**: URL.
	- This parameter is key element.
- **Info**
	- **Data Type**: string
	- **Description**: APIs available under this URL or details of the specific API.


**Flexswitch API Supported:**
	- GET By Key
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://device-management-IP:8080/public/v1/state/ApiInfo


