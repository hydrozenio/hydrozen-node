# HydrozenApi.StatusPageStatisticsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStatusPageStatistics**](StatusPageStatisticsApi.md#getStatusPageStatistics) | **GET** /statistics/{status_page_id} | Retrieve status page statistics



## getStatusPageStatistics

> GetStatusPageStatistics200Response getStatusPageStatistics(statusPageId, startDate, endDate, opts)

Retrieve status page statistics

Returns analytics data for a specific status page based on date range and filters.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.StatusPageStatisticsApi();
let statusPageId = 56; // Number | 
let startDate = new Date("2013-10-20"); // Date | 
let endDate = new Date("2013-10-20"); // Date | 
let opts = {
  'type': "type_example", // String | 
  'countryCode': "countryCode_example", // String | 
  'utmSource': "utmSource_example", // String | 
  'utmMedium': "utmMedium_example" // String | 
};
apiInstance.getStatusPageStatistics(statusPageId, startDate, endDate, opts, (error, data, response) => {
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
 **statusPageId** | **Number**|  | 
 **startDate** | **Date**|  | 
 **endDate** | **Date**|  | 
 **type** | **String**|  | [optional] 
 **countryCode** | **String**|  | [optional] 
 **utmSource** | **String**|  | [optional] 
 **utmMedium** | **String**|  | [optional] 

### Return type

[**GetStatusPageStatistics200Response**](GetStatusPageStatistics200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

