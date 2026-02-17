# mercatorio-js.DefaultApi

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
import mercatorio-js from 'mercatorio.js';
let defaultClient = mercatorio-js.ApiClient.instance;
// Configure API key authorization: X-Merc-User
let X-Merc-User = defaultClient.authentications['X-Merc-User'];
X-Merc-User.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//X-Merc-User.apiKeyPrefix = 'Token';
// Configure API key authorization: Bearer-Token
let Bearer-Token = defaultClient.authentications['Bearer-Token'];
Bearer-Token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer-Token.apiKeyPrefix = 'Token';

let apiInstance = new mercatorio-js.DefaultApi();
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

[X-Merc-User](../README.md#X-Merc-User), [Bearer-Token](../README.md#Bearer-Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## playerInfo

> Player playerInfo()

Get the player information

### Example

```javascript
import mercatorio-js from 'mercatorio.js';
let defaultClient = mercatorio-js.ApiClient.instance;
// Configure API key authorization: X-Merc-User
let X-Merc-User = defaultClient.authentications['X-Merc-User'];
X-Merc-User.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//X-Merc-User.apiKeyPrefix = 'Token';
// Configure API key authorization: Bearer-Token
let Bearer-Token = defaultClient.authentications['Bearer-Token'];
Bearer-Token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer-Token.apiKeyPrefix = 'Token';

let apiInstance = new mercatorio-js.DefaultApi();
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

[X-Merc-User](../README.md#X-Merc-User), [Bearer-Token](../README.md#Bearer-Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

