# HydrozenApi.UptimeMonitorsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**monitorsGet**](UptimeMonitorsApi.md#monitorsGet) | **GET** /monitors | Retrieve all uptime monitors
[**monitorsPost**](UptimeMonitorsApi.md#monitorsPost) | **POST** /monitors | Create uptime monitor



## monitorsGet

> MonitorsGet200Response monitorsGet(opts)

Retrieve all uptime monitors

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.UptimeMonitorsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.monitorsGet(opts, (error, data, response) => {
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

[**MonitorsGet200Response**](MonitorsGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## monitorsPost

> MonitorsPost201Response monitorsPost(name, target, opts)

Create uptime monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.UptimeMonitorsApi();
let name = "name_example"; // String | 
let target = "target_example"; // String | 
let opts = {
  'port': 56, // Number | 
  'type': "type_example", // String | 
  'projectId': 56 // Number | 
};
apiInstance.monitorsPost(name, target, opts, (error, data, response) => {
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
 **name** | **String**|  | 
 **target** | **String**|  | 
 **port** | **Number**|  | [optional] 
 **type** | **String**|  | [optional] 
 **projectId** | **Number**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

