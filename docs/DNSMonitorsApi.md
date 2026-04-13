# HydrozenApi.DNSMonitorsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteDNSMonitor**](DNSMonitorsApi.md#deleteDNSMonitor) | **DELETE** /dns-monitors/{id} | Delete DNS monitor
[**getAllDNSMonitors**](DNSMonitorsApi.md#getAllDNSMonitors) | **GET** /dns-monitors | Retrieve all DNS monitors
[**getDNSMonitor**](DNSMonitorsApi.md#getDNSMonitor) | **GET** /dns-monitors/{id} | Retrieve one DNS monitor



## deleteDNSMonitor

> DeleteDNSMonitor200Response deleteDNSMonitor(id)

Delete DNS monitor

Deletes a DNS monitor.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DNSMonitorsApi();
let id = 56; // Number | 
apiInstance.deleteDNSMonitor(id, (error, data, response) => {
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
 **id** | **Number**|  | 

### Return type

[**DeleteDNSMonitor200Response**](DeleteDNSMonitor200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAllDNSMonitors

> GetAllDNSMonitors200Response getAllDNSMonitors(opts)

Retrieve all DNS monitors

Returns a paginated list of DNS monitors.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DNSMonitorsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.getAllDNSMonitors(opts, (error, data, response) => {
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

[**GetAllDNSMonitors200Response**](GetAllDNSMonitors200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDNSMonitor

> GetDNSMonitor200Response getDNSMonitor(id)

Retrieve one DNS monitor

Returns details of a specific DNS monitor.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DNSMonitorsApi();
let id = 56; // Number | 
apiInstance.getDNSMonitor(id, (error, data, response) => {
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
 **id** | **Number**|  | 

### Return type

[**GetDNSMonitor200Response**](GetDNSMonitor200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

