# MmGatewayJs.VideoRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input** | [**[InputInner2]**](InputInner2.md) | Non-empty ordered video-generation inputs. | 
**metadata** | **{String: Object}** | Client-owned metadata returned unchanged with the task. | [optional] 
**model** | **String** | Model id returned by GET /v1/models, or omit / set to &#x60;auto&#x60; to let the gateway auto-route to a backend whose limits fit the request&#39;s input (modalities, dimensions, duration, ...). | [optional] 
**parameters** | [**VideoParameters**](VideoParameters.md) |  | [optional] 
**routing** | [**RoutingDirective**](RoutingDirective.md) |  | [optional] 


