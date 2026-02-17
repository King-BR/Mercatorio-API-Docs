# mercatoriojs.DefaultApi

All URIs are relative to *https://play.mercatorio.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**buildingInfo**](DefaultApi.md#buildingInfo) | **GET** /buildings/{buildingID} | Get the building information
[**businessInfo**](DefaultApi.md#businessInfo) | **GET** /businesses/{businessID} | Get the business information
[**mapRegions**](DefaultApi.md#mapRegions) | **GET** /map/regions | Get the list of all regions on the map, with their corresponding information
[**playerInfo**](DefaultApi.md#playerInfo) | **GET** /player | Get the player information
[**townInfo**](DefaultApi.md#townInfo) | **GET** /towns/{townID} | Get the information for a specific town
[**towns**](DefaultApi.md#towns) | **GET** /towns | Get the list of all towns on the map, with their corresponding information



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


## businessInfo

> Business businessInfo(businessID)

Get the business information

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
let businessID = "businessID_example"; // String | 
apiInstance.businessInfo(businessID, (error, data, response) => {
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
 **businessID** | **String**|  | 

### Return type

[**Business**](Business.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## mapRegions

> [MapRegion] mapRegions()

Get the list of all regions on the map, with their corresponding information

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
apiInstance.mapRegions((error, data, response) => {
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

[**[MapRegion]**](MapRegion.md)

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


## townInfo

> Town townInfo(townID)

Get the information for a specific town

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
let townID = "townID_example"; // String | 
apiInstance.townInfo(townID, (error, data, response) => {
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
 **townID** | **String**|  | 

### Return type

[**Town**](Town.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## towns

> [TownSimple] towns()

Get the list of all towns on the map, with their corresponding information

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
apiInstance.towns((error, data, response) => {
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

[**[TownSimple]**](TownSimple.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

