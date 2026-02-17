# DefaultApi

All URIs are relative to *https://play.mercatorio.io/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**buildingInfo**](DefaultApi.md#buildingInfo) | **GET** /buildings/{buildingID} | Get the building information |
| [**businessInfo**](DefaultApi.md#businessInfo) | **GET** /businesses/{businessID} | Get the business information |
| [**mapRegions**](DefaultApi.md#mapRegions) | **GET** /map/regions | Get the list of all regions on the map, with their corresponding information |
| [**playerInfo**](DefaultApi.md#playerInfo) | **GET** /player | Get the player information |
| [**townInfo**](DefaultApi.md#townInfo) | **GET** /towns/{townID} | Get the information for a specific town |
| [**towns**](DefaultApi.md#towns) | **GET** /towns | Get the list of all towns on the map, with their corresponding information |


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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

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

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The building corresponding to the buildingID used |  -  |
| **404** | No building found |  -  |
| **500** | Unexpected error |  -  |

<a id="businessInfo"></a>
# **businessInfo**
> Business businessInfo(businessID)

Get the business information

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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String businessID = "businessID_example"; // String | 
    try {
      Business result = apiInstance.businessInfo(businessID);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#businessInfo");
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
| **businessID** | **String**|  | |

### Return type

[**Business**](Business.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The business corresponding to the businessID used |  -  |
| **404** | No business found |  -  |
| **500** | Unexpected error |  -  |

<a id="mapRegions"></a>
# **mapRegions**
> List&lt;MapRegion&gt; mapRegions()

Get the list of all regions on the map, with their corresponding information

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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      List<MapRegion> result = apiInstance.mapRegions();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#mapRegions");
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

[**List&lt;MapRegion&gt;**](MapRegion.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The list of all regions on the map, with their corresponding information |  -  |
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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

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

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The player corresponding to the API key used |  -  |
| **404** | No player found |  -  |
| **500** | Unexpected error |  -  |

<a id="townInfo"></a>
# **townInfo**
> Town townInfo(townID)

Get the information for a specific town

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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String townID = "townID_example"; // String | 
    try {
      Town result = apiInstance.townInfo(townID);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#townInfo");
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
| **townID** | **String**|  | |

### Return type

[**Town**](Town.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The information for a specific town |  -  |
| **404** | No town found |  -  |
| **500** | Unexpected error |  -  |

<a id="towns"></a>
# **towns**
> List&lt;TownSimple&gt; towns()

Get the list of all towns on the map, with their corresponding information

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
    
    // Configure API key authorization: Merc_User
    ApiKeyAuth Merc_User = (ApiKeyAuth) defaultClient.getAuthentication("Merc_User");
    Merc_User.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Merc_User.setApiKeyPrefix("Token");

    // Configure API key authorization: Bearer_Token
    ApiKeyAuth Bearer_Token = (ApiKeyAuth) defaultClient.getAuthentication("Bearer_Token");
    Bearer_Token.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //Bearer_Token.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      List<TownSimple> result = apiInstance.towns();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#towns");
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

[**List&lt;TownSimple&gt;**](TownSimple.md)

### Authorization

[Merc_User](../README.md#Merc_User), [Bearer_Token](../README.md#Bearer_Token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The list of all towns on the map, with their corresponding information |  -  |
| **500** | Unexpected error |  -  |

