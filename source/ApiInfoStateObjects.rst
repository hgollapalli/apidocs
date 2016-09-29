ApiInfoState Model Objects
============================================

*state/ApiInfo*
------------------------------------

- **Url**
	- **Data Type**: string
	- **Description**: URL.
	- This parameter is key element.
- **Info**
	- **Data Type**: string
	- **Description**: APIs available under this URL or details of the specific API.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/ApiInfo


