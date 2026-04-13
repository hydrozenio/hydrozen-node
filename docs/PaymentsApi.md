# HydrozenApi.PaymentsApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAllPayments**](PaymentsApi.md#getAllPayments) | **GET** /payments | Retrieve all payments
[**getPayment**](PaymentsApi.md#getPayment) | **GET** /payments/{payment_id} | Retrieve one payment



## getAllPayments

> GetAllPayments200Response getAllPayments(opts)

Retrieve all payments

Returns a paginated list of payments.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.PaymentsApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.getAllPayments(opts, (error, data, response) => {
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

[**GetAllPayments200Response**](GetAllPayments200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPayment

> GetPayment200Response getPayment(paymentId)

Retrieve one payment

Returns details of a specific payment.

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.PaymentsApi();
let paymentId = 56; // Number | 
apiInstance.getPayment(paymentId, (error, data, response) => {
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
 **paymentId** | **Number**|  | 

### Return type

[**GetPayment200Response**](GetPayment200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

