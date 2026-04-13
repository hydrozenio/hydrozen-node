# HydrozenApi.UsersApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getUser**](UsersApi.md#getUser) | **GET** /user | Retrieve current user



## getUser

> GetUser200Response getUser()

Retrieve current user

Returns details of the authenticated user.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.UsersApi();
apiInstance.getUser((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetUser200Response**](GetUser200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

