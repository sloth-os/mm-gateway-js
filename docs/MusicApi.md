# MmGatewayJs.MusicApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createMusic**](MusicApi.md#createMusic) | **POST** /v1/music | Create a music task
[**getMusic**](MusicApi.md#getMusic) | **GET** /v1/music/{music_id} | Retrieve a music task



## createMusic

> MusicTaskResponse createMusic(musicRequest, opts)

Create a music task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.MusicApi();
let musicRequest = new MmGatewayJs.MusicRequest(); // MusicRequest | 
let opts = {
  'idempotencyKey': "idempotencyKey_example" // String | Client-generated key used to safely retry this create request. Reuse with a different body returns 409.
};
apiInstance.createMusic(musicRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **musicRequest** | [**MusicRequest**](MusicRequest.md)|  | 
 **idempotencyKey** | **String**| Client-generated key used to safely retry this create request. Reuse with a different body returns 409. | [optional] 

### Return type

[**MusicTaskResponse**](MusicTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json


## getMusic

> MusicTaskResponse getMusic(musicId, opts)

Retrieve a music task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.MusicApi();
let musicId = "musicId_example"; // String | Opaque music task id.
let opts = {
  'ifNoneMatch': "ifNoneMatch_example" // String | Previously returned ETag; unchanged resources return 304.
};
apiInstance.getMusic(musicId, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **musicId** | **String**| Opaque music task id. | 
 **ifNoneMatch** | **String**| Previously returned ETag; unchanged resources return 304. | [optional] 

### Return type

[**MusicTaskResponse**](MusicTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

