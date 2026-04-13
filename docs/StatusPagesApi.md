# HydrozenApi.StatusPagesApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAllStatusPages**](StatusPagesApi.md#getAllStatusPages) | **GET** /status-pages | Retrieve all status pages
[**getStatusPage**](StatusPagesApi.md#getStatusPage) | **GET** /status-pages/{status_page_id} | Retrieve one status page



## getAllStatusPages

> GetAllStatusPages200Response getAllStatusPages(opts)

Retrieve all status pages

Returns a paginated list of status pages.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.StatusPagesApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.getAllStatusPages(opts, (error, data, response) => {
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
 **page** | **Number**|  | [optional] 
 **resultsPerPage** | **Number**|  | [optional] 

### Return type

[**GetAllStatusPages200Response**](GetAllStatusPages200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getStatusPage

> GetStatusPage200Response getStatusPage(statusPageId)

Retrieve one status page

Returns details of a specific status page.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.StatusPagesApi();
let statusPageId = 56; // Number | 
apiInstance.getStatusPage(statusPageId, (error, data, response) => {
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

### Return type

[**GetStatusPage200Response**](GetStatusPage200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

