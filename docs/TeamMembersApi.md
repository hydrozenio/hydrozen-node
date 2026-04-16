# HydrozenApi.TeamMembersApi

All URIs are relative to *https://app.hydrozen.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTeamMember**](TeamMembersApi.md#createTeamMember) | **POST** /team-members | Create team member
[**deleteTeamMember**](TeamMembersApi.md#deleteTeamMember) | **DELETE** /team-members/{team_member_id} | Delete team member
[**getTeamMembersByTeam**](TeamMembersApi.md#getTeamMembersByTeam) | **GET** /team-members/{team_id} | Retrieve team members
[**updateTeamMember**](TeamMembersApi.md#updateTeamMember) | **POST** /team-members/{team_member_id} | Update team member



## createTeamMember

> MonitorsPost201Response createTeamMember(teamId, userEmail, opts)

Create team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.TeamMembersApi();
let teamId = 56; // Number | 
let userEmail = "userEmail_example"; // String | 
let opts = {
  'access': ["null"] // [String] | 
};
apiInstance.createTeamMember(teamId, userEmail, opts, (error, data, response) => {
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
 **teamId** | **Number**|  | 
 **userEmail** | **String**|  | 
 **access** | [**[String]**](String.md)|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## deleteTeamMember

> deleteTeamMember(teamMemberId)

Delete team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.TeamMembersApi();
let teamMemberId = 56; // Number | 
apiInstance.deleteTeamMember(teamMemberId, (error, data, response) => {
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


## getTeamMembersByTeam

> GetTeamMembersByTeam200Response getTeamMembersByTeam(teamId)

Retrieve team members

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.TeamMembersApi();
let teamId = 56; // Number | 
apiInstance.getTeamMembersByTeam(teamId, (error, data, response) => {
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
 **teamId** | **Number**|  | 

### Return type

[**GetTeamMembersByTeam200Response**](GetTeamMembersByTeam200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTeamMember

> MonitorsPost201Response updateTeamMember(teamMemberId, opts)

Update team member

### Example

```javascript
import HydrozenApi from 'hydrozen_api';
let defaultClient = HydrozenApi.ApiClient.instance;
// Configure Bearer (API Key) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new HydrozenApi.TeamMembersApi();
let teamMemberId = 56; // Number | 
let opts = {
  'access': ["null"] // [String] | 
};
apiInstance.updateTeamMember(teamMemberId, opts, (error, data, response) => {
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
 **access** | [**[String]**](String.md)|  | [optional] 

### Return type

[**MonitorsPost201Response**](MonitorsPost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

