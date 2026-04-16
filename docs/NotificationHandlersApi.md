# HydrozenApi.NotificationHandlersApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**notificationHandlerGet**](NotificationHandlersApi.md#notificationHandlerGet) | **GET** /notification-handler | Retrieve all notification handlers
[**notificationHandlerNotificationHandlerIdGet**](NotificationHandlersApi.md#notificationHandlerNotificationHandlerIdGet) | **GET** /notification-handler/{notification_handler_id} | Retrieve one notification handler
[**notificationHandlersNotificationHandlerIdDelete**](NotificationHandlersApi.md#notificationHandlersNotificationHandlerIdDelete) | **DELETE** /notification-handlers/{notification_handler_id} | Delete notification handler
[**notificationHandlersNotificationHandlerIdPost**](NotificationHandlersApi.md#notificationHandlersNotificationHandlerIdPost) | **POST** /notification-handlers/{notification_handler_id} | Update notification handler
[**notificationHandlersPost**](NotificationHandlersApi.md#notificationHandlersPost) | **POST** /notification-handlers | Create notification handler



## notificationHandlerGet

> NotificationHandlerGet200Response notificationHandlerGet(opts)

Retrieve all notification handlers

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.NotificationHandlersApi();
let opts = {
  'page': 56, // Number | 
  'resultsPerPage': 56 // Number | 
};
apiInstance.notificationHandlerGet(opts, (error, data, response) => {
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

[**NotificationHandlerGet200Response**](NotificationHandlerGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## notificationHandlerNotificationHandlerIdGet

> NotificationHandlerNotificationHandlerIdGet200Response notificationHandlerNotificationHandlerIdGet(notificationHandlerId)

Retrieve one notification handler

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.NotificationHandlersApi();
let notificationHandlerId = 56; // Number | 
apiInstance.notificationHandlerNotificationHandlerIdGet(notificationHandlerId, (error, data, response) => {
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
 **notificationHandlerId** | **Number**|  | 

### Return type

[**NotificationHandlerNotificationHandlerIdGet200Response**](NotificationHandlerNotificationHandlerIdGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## notificationHandlersNotificationHandlerIdDelete

> notificationHandlersNotificationHandlerIdDelete(notificationHandlerId)

Delete notification handler

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.NotificationHandlersApi();
let notificationHandlerId = 56; // Number | 
apiInstance.notificationHandlersNotificationHandlerIdDelete(notificationHandlerId, (error, data, response) => {
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
 **notificationHandlerId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## notificationHandlersNotificationHandlerIdPost

> MonitorsPost201Response notificationHandlersNotificationHandlerIdPost(notificationHandlerId, opts)

Update notification handler

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.NotificationHandlersApi();
let notificationHandlerId = 56; // Number | 
let opts = {
  'name': "name_example", // String | 
  'type': "type_example", // String | 
  'email': "email_example", // String | 
  'webhook': "webhook_example", // String | 
  'squadcast': "squadcast_example", // String | 
  'googlechat': "googlechat_example", // String | 
  'slack': "slack_example", // String | 
  'discord': "discord_example", // String | 
  'telegram': "telegram_example", // String | 
  'telegramChatId': "telegramChatId_example", // String | 
  'isEnabled': true // Boolean | 
};
apiInstance.notificationHandlersNotificationHandlerIdPost(notificationHandlerId, opts, (error, data, response) => {
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
 **notificationHandlerId** | **Number**|  | 
 **name** | **String**|  | [optional] 
 **type** | **String**|  | [optional] 
 **email** | **String**|  | [optional] 
 **webhook** | **String**|  | [optional] 
 **squadcast** | **String**|  | [optional] 
 **googlechat** | **String**|  | [optional] 
 **slack** | **String**|  | [optional] 
 **discord** | **String**|  | [optional] 
 **telegram** | **String**|  | [optional] 
 **telegramChatId** | **String**|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## notificationHandlersPost

> MonitorsPost201Response notificationHandlersPost(name, type, opts)

Create notification handler

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.NotificationHandlersApi();
let name = "name_example"; // String | 
let type = "type_example"; // String | 
let opts = {
  'email': "email_example", // String | 
  'webhook': "webhook_example", // String | 
  'squadcast': "squadcast_example", // String | 
  'googlechat': "googlechat_example", // String | 
  'slack': "slack_example", // String | 
  'discord': "discord_example", // String | 
  'telegram': "telegram_example", // String | 
  'telegramChatId': "telegramChatId_example", // String | 
  'isEnabled': true // Boolean | 
};
apiInstance.notificationHandlersPost(name, type, opts, (error, data, response) => {
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
 **type** | **String**|  | 
 **email** | **String**|  | [optional] 
 **webhook** | **String**|  | [optional] 
 **squadcast** | **String**|  | [optional] 
 **googlechat** | **String**|  | [optional] 
 **slack** | **String**|  | [optional] 
 **discord** | **String**|  | [optional] 
 **telegram** | **String**|  | [optional] 
 **telegramChatId** | **String**|  | [optional] 
 **isEnabled** | **Boolean**|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

