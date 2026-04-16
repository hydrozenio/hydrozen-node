# HydrozenApi.DomainMonitorsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**domainNamesDomainNameIdDelete**](DomainMonitorsApi.md#domainNamesDomainNameIdDelete) | **DELETE** /domain-names/{domain_name_id} | Delete domain name monitor
[**domainNamesDomainNameIdGet**](DomainMonitorsApi.md#domainNamesDomainNameIdGet) | **GET** /domain-names/{domain_name_id} | Retrieve one domain name monitor
[**domainNamesDomainNameIdPost**](DomainMonitorsApi.md#domainNamesDomainNameIdPost) | **POST** /domain-names/{domain_name_id} | Update domain name monitor
[**domainNamesGet**](DomainMonitorsApi.md#domainNamesGet) | **GET** /domain-names | Retrieve all domain name monitors
[**domainNamesPost**](DomainMonitorsApi.md#domainNamesPost) | **POST** /domain-names | Create domain name monitor



## domainNamesDomainNameIdDelete

> domainNamesDomainNameIdDelete(domainNameId)

Delete domain name monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DomainMonitorsApi();
let domainNameId = 56; // Number | 
apiInstance.domainNamesDomainNameIdDelete(domainNameId, (error, data, response) => {
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
 **domainNameId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## domainNamesDomainNameIdGet

> DomainNamesDomainNameIdGet200Response domainNamesDomainNameIdGet(domainNameId)

Retrieve one domain name monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DomainMonitorsApi();
let domainNameId = 56; // Number | 
apiInstance.domainNamesDomainNameIdGet(domainNameId, (error, data, response) => {
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
 **domainNameId** | **Number**|  | 

### Return type

[**DomainNamesDomainNameIdGet200Response**](DomainNamesDomainNameIdGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## domainNamesDomainNameIdPost

> MonitorsPost201Response domainNamesDomainNameIdPost(domainNameId, opts)

Update domain name monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DomainMonitorsApi();
let domainNameId = 56; // Number | 
let opts = {
  'name': "name_example", // String | 
  'target': "target_example", // String | 
  'projectId': 56, // Number | 
  'whoisNotifications': [null], // [Number] | 
  'whoisNotificationsTiming': 56, // Number | 
  'sslNotifications': [null], // [Number] | 
  'sslNotificationsTiming': 56, // Number | 
  'isEnabled': true // Boolean | 
};
apiInstance.domainNamesDomainNameIdPost(domainNameId, opts, (error, data, response) => {
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
 **domainNameId** | **Number**|  | 
 **name** | **String**|  | [optional] 
 **target** | **String**|  | [optional] 
 **projectId** | **Number**|  | [optional] 
 **whoisNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **whoisNotificationsTiming** | **Number**|  | [optional] 
 **sslNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **sslNotificationsTiming** | **Number**|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## domainNamesGet

> DomainNamesGet200Response domainNamesGet(opts)

Retrieve all domain name monitors

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DomainMonitorsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.domainNamesGet(opts, (error, data, response) => {
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

[**DomainNamesGet200Response**](DomainNamesGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## domainNamesPost

> MonitorsPost201Response domainNamesPost(name, target, opts)

Create domain name monitor

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.DomainMonitorsApi();
let name = "name_example"; // String | 
let target = "target_example"; // String | 
let opts = {
  'projectId': 56, // Number | 
  'whoisNotifications': [null], // [Number] | 
  'whoisNotificationsTiming': 56, // Number | 
  'sslNotifications': [null], // [Number] | 
  'sslNotificationsTiming': 56, // Number | 
  'isEnabled': true // Boolean | 
};
apiInstance.domainNamesPost(name, target, opts, (error, data, response) => {
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
 **projectId** | **Number**|  | [optional] 
 **whoisNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **whoisNotificationsTiming** | **Number**|  | [optional] 
 **sslNotifications** | [**[Number]**](Number.md)|  | [optional] 
 **sslNotificationsTiming** | **Number**|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

