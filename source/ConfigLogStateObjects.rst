ConfigLogState Model Objects
============================================

*state/ConfigLog*
------------------------------------

- **SeqNum**
	- **Data Type**: uint32
	- **Description**: Sequence number of the API call.
	- This parameter is key element.
- **Time**
	- **Data Type**: string
	- **Description**: When the API was called.
	- This parameter is key element.
- **API**
	- **Data Type**: string
	- **Description**: Name of the API called.
	- This parameter is key element.
- **Result**
	- **Data Type**: string
	- **Description**: Result of the API call.
- **UserAddr**
	- **Data Type**: string
	- **Description**: Host address from where the call was made.
- **UserName**
	- **Data Type**: string
	- **Description**: User who made the call.
- **Data**
	- **Data Type**: string
	- **Description**: User provided data.
- **Operation**
	- **Data Type**: string
	- **Description**: Oprtation executed on this API.


**REST API Supported:**
	- GET
		 curl -X GET -H 'Content-Type: application/json' --header 'Accept: application/json' -d '{<Model Object as json-Data>}' http://<device-management-IP>:8080/public/v1/state/ConfigLog


