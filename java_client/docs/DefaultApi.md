# DefaultApi

All URIs are relative to *https://play.mercatorio.io/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**buildingInfo**](DefaultApi.md#buildingInfo) | **GET** /buildings/{buildingID} | Get the building information |
| [**playerInfo**](DefaultApi.md#playerInfo) | **GET** /player | Get the player information |


<a id="buildingInfo"></a>
# **buildingInfo**
> Building buildingInfo(buildingID)

Get the building information

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://play.mercatorio.io/api");
    
    // Configure API key authorization: X-Merc-User
    ApiKeyAuth X-Merc-User = (ApiKeyAuth) defaultClient.getAuthentication("X-Merc-User");
    X-Merc-User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //X-Merc-User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer-Token
    ApiKeyAuth Bearer-Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer-Token");
    Bearer-Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer-Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String buildingID = "buildingID_example"; // String | 
    try {
      Building result = apiInstance.buildingInfo(buildingID);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#buildingInfo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **buildingID** | **String**|  | |

### Return type

[**Building**](Building.md)

### Authorization

[X-Merc-User](../README.md#X-Merc-User), [Bearer-Token](../README.md#Bearer-Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The building corresponding to the buildingID used |  -  |
| **404** | No building found |  -  |
| **500** | Unexpected error |  -  |

<a id="playerInfo"></a>
# **playerInfo**
> Player playerInfo()

Get the player information

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://play.mercatorio.io/api");
    
    // Configure API key authorization: X-Merc-User
    ApiKeyAuth X-Merc-User = (ApiKeyAuth) defaultClient.getAuthentication("X-Merc-User");
    X-Merc-User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //X-Merc-User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer-Token
    ApiKeyAuth Bearer-Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer-Token");
    Bearer-Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer-Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      Player result = apiInstance.playerInfo();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#playerInfo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
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

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The player corresponding to the API key used |  -  |
| **404** | No player found |  -  |
| **500** | Unexpected error |  -  |

