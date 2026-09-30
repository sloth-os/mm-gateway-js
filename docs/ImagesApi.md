# MmGatewayJs.ImagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createImage**](ImagesApi.md#createImage) | **POST** /v1/images | Create an image task
[**getImage**](ImagesApi.md#getImage) | **GET** /v1/images/{image_id} | Retrieve an image task



## createImage

> ImageTaskResponse createImage(imageRequest, opts)

Create an image task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ImagesApi();
let imageRequest = new MmGatewayJs.ImageRequest(); // ImageRequest | 
let opts = {
  'idempotencyKey': "idempotencyKey_example" // String | Client-generated key used to safely retry this create request. Reuse with a different body returns 409.
};
apiInstance.createImage(imageRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **imageRequest** | [**ImageRequest**](ImageRequest.md)|  | 
 **idempotencyKey** | **String**| Client-generated key used to safely retry this create request. Reuse with a different body returns 409. | [optional] 

### Return type

[**ImageTaskResponse**](ImageTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json


## getImage

> ImageTaskResponse getImage(imageId, opts)

Retrieve an image task

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ImagesApi();
let imageId = "imageId_example"; // String | Opaque image task id.
let opts = {
  'ifNoneMatch': "ifNoneMatch_example" // String | Previously returned ETag; unchanged resources return 304.
};
apiInstance.getImage(imageId, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **imageId** | **String**| Opaque image task id. | 
 **ifNoneMatch** | **String**| Previously returned ETag; unchanged resources return 304. | [optional] 

### Return type

[**ImageTaskResponse**](ImageTaskResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

