# HydrozenApi.CustomDomainsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCustomDomain**](CustomDomainsApi.md#createCustomDomain) | **POST** /domains | Create custom domain
[**deleteCustomDomain**](CustomDomainsApi.md#deleteCustomDomain) | **DELETE** /domains/{domain_id} | Delete custom domain
[**getAllCustomDomains**](CustomDomainsApi.md#getAllCustomDomains) | **GET** /domains | Retrieve all custom domains
[**getCustomDomain**](CustomDomainsApi.md#getCustomDomain) | **GET** /domains/{domain_id} | Retrieve one custom domain
[**updateCustomDomain**](CustomDomainsApi.md#updateCustomDomain) | **POST** /domains/{domain_id} | Update custom domain



## createCustomDomain

> MonitorsPost201Response createCustomDomain(host, opts)

Create custom domain

Creates a new custom domain.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.CustomDomainsApi();
let host = "host_example"; // String | 
let opts = {
  'customIndexUrl': "customIndexUrl_example", // String | 
  'customNotFoundUrl': "customNotFoundUrl_example" // String | 
};
apiInstance.createCustomDomain(host, opts, (error, data, response) => {
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
 **host** | **String**|  | 
 **customIndexUrl** | **String**|  | [optional] 
 **customNotFoundUrl** | **String**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## deleteCustomDomain

> deleteCustomDomain(domainId)

Delete custom domain

Deletes a custom domain.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.CustomDomainsApi();
let domainId = 56; // Number | 
apiInstance.deleteCustomDomain(domainId, (error, data, response) => {
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
 **domainId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllCustomDomains

> GetAllCustomDomains200Response getAllCustomDomains(opts)

Retrieve all custom domains

Returns a paginated list of custom domains.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.CustomDomainsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.getAllCustomDomains(opts, (error, data, response) => {
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

[**GetAllCustomDomains200Response**](GetAllCustomDomains200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCustomDomain

> GetCustomDomain200Response getCustomDomain(domainId)

Retrieve one custom domain

Returns details of a specific custom domain.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.CustomDomainsApi();
let domainId = 56; // Number | 
apiInstance.getCustomDomain(domainId, (error, data, response) => {
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
 **domainId** | **Number**|  | 

### Return type

[**GetCustomDomain200Response**](GetCustomDomain200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCustomDomain

> MonitorsPost201Response updateCustomDomain(domainId, opts)

Update custom domain

Updates an existing custom domain.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.CustomDomainsApi();
let domainId = 56; // Number | 
let opts = {
  'host': "host_example", // String | 
  'customIndexUrl': "customIndexUrl_example", // String | 
  'customNotFoundUrl': "customNotFoundUrl_example" // String | 
};
apiInstance.updateCustomDomain(domainId, opts, (error, data, response) => {
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
 **domainId** | **Number**|  | 
 **host** | **String**|  | [optional] 
 **customIndexUrl** | **String**|  | [optional] 
 **customNotFoundUrl** | **String**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

