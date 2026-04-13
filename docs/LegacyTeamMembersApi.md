# HydrozenApi.LegacyTeamMembersApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteTeamMemberLegacy**](LegacyTeamMembersApi.md#deleteTeamMemberLegacy) | **DELETE** /teams-member/{team_member_id} | Delete team member
[**getAllTeamMembersLegacy**](LegacyTeamMembersApi.md#getAllTeamMembersLegacy) | **GET** /teams-member | Retrieve all team members
[**getTeamMemberLegacy**](LegacyTeamMembersApi.md#getTeamMemberLegacy) | **GET** /teams-member/{team_member_id} | Retrieve one team member
[**updateTeamMemberLegacy**](LegacyTeamMembersApi.md#updateTeamMemberLegacy) | **POST** /teams-member/{team_member_id} | Update team member



## deleteTeamMemberLegacy

> deleteTeamMemberLegacy(teamMemberId)

Delete team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.LegacyTeamMembersApi();
let teamMemberId = 56; // Number | 
apiInstance.deleteTeamMemberLegacy(teamMemberId, (error, data, response) => {
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
 **teamMemberId** | **Number**|  | 

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllTeamMembersLegacy

> GetAllTeamMembersLegacy200Response getAllTeamMembersLegacy(opts)

Retrieve all team members

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.LegacyTeamMembersApi();
let opts = {
  'page': 1, // Number | 
  'resultsPerPage': 25 // Number | 
};
apiInstance.getAllTeamMembersLegacy(opts, (error, data, response) => {
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
 **page** | **Number**|  | [optional] [default to 1]
 **resultsPerPage** | **Number**|  | [optional] [default to 25]

### Return type

[**GetAllTeamMembersLegacy200Response**](GetAllTeamMembersLegacy200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTeamMemberLegacy

> GetTeamMemberLegacy200Response getTeamMemberLegacy(teamMemberId)

Retrieve one team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.LegacyTeamMembersApi();
let teamMemberId = 56; // Number | 
apiInstance.getTeamMemberLegacy(teamMemberId, (error, data, response) => {
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
 **teamMemberId** | **Number**|  | 

### Return type

[**GetTeamMemberLegacy200Response**](GetTeamMemberLegacy200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTeamMemberLegacy

> MonitorsPost201Response updateTeamMemberLegacy(teamMemberId, opts)

Update team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.LegacyTeamMembersApi();
let teamMemberId = 56; // Number | 
let opts = {
  'status': true // Boolean | Enable or disable team member
};
apiInstance.updateTeamMemberLegacy(teamMemberId, opts, (error, data, response) => {
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
 **teamMemberId** | **Number**|  | 
 **status** | **Boolean**| Enable or disable team member | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

