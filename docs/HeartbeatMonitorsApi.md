# HydrozenApi.HeartbeatMonitorsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**heartbeatsGet**](HeartbeatMonitorsApi.md#heartbeatsGet) | **GET** /heartbeats | Retrieve all heartbeat monitors
[**heartbeatsHeartbeatIdDelete**](HeartbeatMonitorsApi.md#heartbeatsHeartbeatIdDelete) | **DELETE** /heartbeats/{heartbeat_id} | Delete heartbeat monitor
[**heartbeatsHeartbeatIdGet**](HeartbeatMonitorsApi.md#heartbeatsHeartbeatIdGet) | **GET** /heartbeats/{heartbeat_id} | Retrieve one heartbeat monitor
[**heartbeatsHeartbeatIdPost**](HeartbeatMonitorsApi.md#heartbeatsHeartbeatIdPost) | **POST** /heartbeats/{heartbeat_id} | Update heartbeat monitor
[**heartbeatsPost**](HeartbeatMonitorsApi.md#heartbeatsPost) | **POST** /heartbeats | Create heartbeat monitor



## heartbeatsGet

> HeartbeatsGet200Response heartbeatsGet(opts)

Retrieve all heartbeat monitors

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.HeartbeatMonitorsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.heartbeatsGet(opts, (error, data, response) => {
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

[**HeartbeatsGet200Response**](HeartbeatsGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## heartbeatsHeartbeatIdDelete

> heartbeatsHeartbeatIdDelete(heartbeatId)

Delete heartbeat monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.HeartbeatMonitorsApi();
let heartbeatId = 56; // Number | 
apiInstance.heartbeatsHeartbeatIdDelete(heartbeatId, (error, data, response) => {
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
 **heartbeatId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## heartbeatsHeartbeatIdGet

> HeartbeatsHeartbeatIdGet200Response heartbeatsHeartbeatIdGet(heartbeatId)

Retrieve one heartbeat monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.HeartbeatMonitorsApi();
let heartbeatId = 56; // Number | 
apiInstance.heartbeatsHeartbeatIdGet(heartbeatId, (error, data, response) => {
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
 **heartbeatId** | **Number**|  | 

### Return type

[**HeartbeatsHeartbeatIdGet200Response**](HeartbeatsHeartbeatIdGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## heartbeatsHeartbeatIdPost

> MonitorsPost201Response heartbeatsHeartbeatIdPost(heartbeatId, opts)

Update heartbeat monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.HeartbeatMonitorsApi();
let heartbeatId = 56; // Number | 
let opts = {
  'name': "name_example", // String | 
  'runInterval': 56, // Number | 
  'runIntervalType': "runIntervalType_example", // String | 
  'runIntervalGrace': 56, // Number | 
  'runIntervalGraceType': "runIntervalGraceType_example", // String | 
  'isOkNotifications': [null], // [Number] | 
  'isEnabled': true // Boolean | 
};
apiInstance.heartbeatsHeartbeatIdPost(heartbeatId, opts, (error, data, response) => {
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
 **heartbeatId** | **Number**|  | 
 **name** | **String**|  | [optional] 
 **runInterval** | **Number**|  | [optional] 
 **runIntervalType** | **String**|  | [optional] 
 **runIntervalGrace** | **Number**|  | [optional] 
 **runIntervalGraceType** | **String**|  | [optional] 
 **isOkNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## heartbeatsPost

> MonitorsPost201Response heartbeatsPost(name, opts)

Create heartbeat monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.HeartbeatMonitorsApi();
let name = "name_example"; // String | 
let opts = {
  'runInterval': 56, // Number | 
  'runIntervalType': "runIntervalType_example", // String | 
  'runIntervalGrace': 56, // Number | 
  'runIntervalGraceType': "runIntervalGraceType_example", // String | 
  'isOkNotifications': [null], // [Number] | 
  'isEnabled': true // Boolean | 
};
apiInstance.heartbeatsPost(name, opts, (error, data, response) => {
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
 **runInterval** | **Number**|  | [optional] 
 **runIntervalType** | **String**|  | [optional] 
 **runIntervalGrace** | **Number**|  | [optional] 
 **runIntervalGraceType** | **String**|  | [optional] 
 **isOkNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

