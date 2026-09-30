# MmGatewayJs.MetaApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getHealth**](MetaApi.md#getHealth) | **GET** /health | Health
[**getMetrics**](MetaApi.md#getMetrics) | **GET** /metrics | Metrics
[**listModelLimits**](MetaApi.md#listModelLimits) | **GET** /v1/models/limits | List Model Limits
[**listModels**](MetaApi.md#listModels) | **GET** /v1/models | List Models



## getHealth

> HealthResponse getHealth()

Health

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';

let apiInstance = new MmGatewayJs.MetaApi();
apiInstance.getHealth().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getMetrics

> String getMetrics()

Metrics

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';

let apiInstance = new MmGatewayJs.MetaApi();
apiInstance.getMetrics().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain


## listModelLimits

> ModelLimitsListResponse listModelLimits(opts)

List Model Limits

List usable models with their documented input/output limits.  Use this to pick a model and craft a prompt that fits: each entry&#39;s &#x60;&#x60;limits&#x60;&#x60; carries the input modalities accepted, the max prompt length, the max output count, supported sizes/durations, and per-role support flags (image-to-image, first/last frame, reference audio, lyrics, ...). The same catalogue drives auto-routing when a request omits &#x60;&#x60;model&#x60;&#x60;.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.MetaApi();
let opts = {
  'modality': "modality_example", // String | Filter models by output modality.
  'authorization': "authorization_example", // String | Bearer token: \"Bearer <api-key>\".
  'xRequestId': "xRequestId_example", // String | Client-supplied request id (echoed back).
  'ifNoneMatch': "ifNoneMatch_example" // String | Previously returned ETag; unchanged resources return 304.
};
apiInstance.listModelLimits(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modality** | **String**| Filter models by output modality. | [optional] 
 **authorization** | **String**| Bearer token: \&quot;Bearer &lt;api-key&gt;\&quot;. | [optional] 
 **xRequestId** | **String**| Client-supplied request id (echoed back). | [optional] 
 **ifNoneMatch** | **String**| Previously returned ETag; unchanged resources return 304. | [optional] 

### Return type

[**ModelLimitsListResponse**](ModelLimitsListResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json


## listModels

> ModelListResponse listModels(opts)

List Models

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.MetaApi();
let opts = {
  'modality': "modality_example", // String | Filter models by output modality.
  'authorization': "authorization_example", // String | Bearer token: \"Bearer <api-key>\".
  'xRequestId': "xRequestId_example", // String | Client-supplied request id (echoed back).
  'ifNoneMatch': "ifNoneMatch_example" // String | Previously returned ETag; unchanged resources return 304.
};
apiInstance.listModels(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **modality** | **String**| Filter models by output modality. | [optional] 
 **authorization** | **String**| Bearer token: \&quot;Bearer &lt;api-key&gt;\&quot;. | [optional] 
 **xRequestId** | **String**| Client-supplied request id (echoed back). | [optional] 
 **ifNoneMatch** | **String**| Previously returned ETag; unchanged resources return 304. | [optional] 

### Return type

[**ModelListResponse**](ModelListResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

