# mercatoriojs.DefaultApi

All URIs are relative to *https://play.mercatorio.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**buildingInfo**](DefaultApi.md#buildingInfo) | **GET** /buildings/{buildingID} | Get the building information
[**playerInfo**](DefaultApi.md#playerInfo) | **GET** /player | Get the player information



## buildingInfo

> Building buildingInfo(buildingID)

Get the building information

### Example

```javascript
import mercatoriojs from 'mercatorio.js';
let defaultClient = mercatoriojs.ApiClient.instance;
// Configure API key authorization: Merc_User
let Merc_User = defaultClient.authentications['Merc_User'];
Merc_User.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Merc_User.apiKeyPrefix = 'Token';
// Configure API key authorization: Bearer_Token
let Bearer_Token = defaultClient.authentications['Bearer_Token'];
Bearer_Token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer_Token.apiKeyPrefix = 'Token';

let apiInstance = new mercatoriojs.DefaultApi();
let buildingID = "buildingID_example"; // String | 
apiInstance.buildingInfo(buildingID, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **buildingID** | **String**|  | 

### Return type

[**Building**](Building.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## playerInfo

> Player playerInfo()

Get the player information

### Example

```javascript
import mercatoriojs from 'mercatorio.js';
let defaultClient = mercatoriojs.ApiClient.instance;
// Configure API key authorization: Merc_User
let Merc_User = defaultClient.authentications['Merc_User'];
Merc_User.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Merc_User.apiKeyPrefix = 'Token';
// Configure API key authorization: Bearer_Token
let Bearer_Token = defaultClient.authentications['Bearer_Token'];
Bearer_Token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer_Token.apiKeyPrefix = 'Token';

let apiInstance = new mercatoriojs.DefaultApi();
apiInstance.playerInfo((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Player**](Player.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

