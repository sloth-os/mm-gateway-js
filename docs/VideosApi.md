# MmGatewayJs.VideosApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createVideo**](VideosApi.md#createVideo) | **POST** /v1/videos | Create a video task
[**getVideo**](VideosApi.md#getVideo) | **GET** /v1/videos/{video_id} | Retrieve a video task



## createVideo

> VideoTaskResponse createVideo(videoRequest, opts)

Create a video task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.VideosApi();
let videoRequest = new MmGatewayJs.VideoRequest(); // VideoRequest | 
let opts = {
  'idempotencyKey': "idempotencyKey_example" // String | Client-generated key used to safely retry this create request. Reuse with a different body returns 409.
};
apiInstance.createVideo(videoRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **videoRequest** | [**VideoRequest**](VideoRequest.md)|  | 
 **idempotencyKey** | **String**| Client-generated key used to safely retry this create request. Reuse with a different body returns 409. | [optional] 

### Return type

[**VideoTaskResponse**](VideoTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json


## getVideo

> VideoTaskResponse getVideo(videoId, opts)

Retrieve a video task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.VideosApi();
let videoId = "videoId_example"; // String | Opaque video task id.
let opts = {
  'ifNoneMatch': "ifNoneMatch_example" // String | Previously returned ETag; unchanged resources return 304.
};
apiInstance.getVideo(videoId, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **videoId** | **String**| Opaque video task id. | 
 **ifNoneMatch** | **String**| Previously returned ETag; unchanged resources return 304. | [optional] 

### Return type

[**VideoTaskResponse**](VideoTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

