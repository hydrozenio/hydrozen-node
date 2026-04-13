# HydrozenApi.ServerMonitorsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteServerMonitor**](ServerMonitorsApi.md#deleteServerMonitor) | **DELETE** /server-monitors/{server_monitor_id} | Delete server monitor
[**getAllServerMonitors**](ServerMonitorsApi.md#getAllServerMonitors) | **GET** /server-monitors | Retrieve all server monitors
[**getServerMonitor**](ServerMonitorsApi.md#getServerMonitor) | **GET** /server-monitors/{server_monitor_id} | Retrieve one server monitor



## deleteServerMonitor

> deleteServerMonitor(serverMonitorId)

Delete server monitor

Deletes a specific server monitor.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.ServerMonitorsApi();
let serverMonitorId = 56; // Number | 
apiInstance.deleteServerMonitor(serverMonitorId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **serverMonitorId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllServerMonitors

> GetAllServerMonitors200Response getAllServerMonitors(opts)

Retrieve all server monitors

Returns a paginated list of server monitors.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.ServerMonitorsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.getAllServerMonitors(opts, (error, data, response) => {
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

[**GetAllServerMonitors200Response**](GetAllServerMonitors200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getServerMonitor

> GetServerMonitor200Response getServerMonitor(serverMonitorId)

Retrieve one server monitor

Returns details of a specific server monitor.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.ServerMonitorsApi();
let serverMonitorId = 56; // Number | 
apiInstance.getServerMonitor(serverMonitorId, (error, data, response) => {
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
 **serverMonitorId** | **Number**|  | 

### Return type

[**GetServerMonitor200Response**](GetServerMonitor200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

