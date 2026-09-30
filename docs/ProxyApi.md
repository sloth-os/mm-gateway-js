# MmGatewayJs.ProxyApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**proxyRequestDelete**](ProxyApi.md#proxyRequestDelete) | **DELETE** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestGet**](ProxyApi.md#proxyRequestGet) | **GET** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestHead**](ProxyApi.md#proxyRequestHead) | **HEAD** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestOptions**](ProxyApi.md#proxyRequestOptions) | **OPTIONS** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestPatch**](ProxyApi.md#proxyRequestPatch) | **PATCH** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestPost**](ProxyApi.md#proxyRequestPost) | **POST** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy
[**proxyRequestPut**](ProxyApi.md#proxyRequestPut) | **PUT** /proxy/{domain}/{path} | Forward a request through a domain-matched proxy



## proxyRequestDelete

> proxyRequestDelete(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestDelete(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestGet

> proxyRequestGet(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestGet(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestHead

> proxyRequestHead(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestHead(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestOptions

> proxyRequestOptions(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestOptions(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestPatch

> proxyRequestPatch(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestPatch(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestPost

> proxyRequestPost(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestPost(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json


## proxyRequestPut

> proxyRequestPut(domain, path)

Forward a request through a domain-matched proxy

Forward an HTTP request through a domain-matched proxy to its upstream.  The path, query string, body, and most client headers are forwarded verbatim to &#x60;&#x60;{base_url}/{path}&#x60;&#x60;; the configured account&#39;s credential is injected from the account&#39;s &#x60;&#x60;headers&#x60;&#x60; and the upstream response (including event streams) is streamed back. Retries across accounts on a rate-limit / timeout / 5xx.

### Example

```javascript
import MmGatewayJs from 'mm-gateway-js';
let defaultClient = MmGatewayJs.ApiClient.instance;
// Configure Bearer (API key) access token for authorization: BearerAuth
let BearerAuth = defaultClient.authentications['BearerAuth'];
BearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MmGatewayJs.ProxyApi();
let domain = "domain_example"; // String | Configured proxy domain (the upstream host segment selecting the proxy).
let path = "path_example"; // String | Path forwarded to the upstream root URL.
apiInstance.proxyRequestPut(domain, path).then(() => {
  console.log('API called successfully.');
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| Configured proxy domain (the upstream host segment selecting the proxy). | 
 **path** | **String**| Path forwarded to the upstream root URL. | 

### Return type

null (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json

