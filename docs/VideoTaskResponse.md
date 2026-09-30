# MmGatewayJs.VideoTaskResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**completedAt** | **Date** |  | [optional] 
**createdAt** | **Date** |  | 
**error** | [**TaskError**](TaskError.md) |  | [optional] 
**id** | **String** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | 
**metadata** | **{String: Object}** |  | [optional] 
**model** | **String** |  | 
**object** | **String** |  | [optional] [default to &#39;video&#39;]
**outputs** | [**[VideoOutput]**](VideoOutput.md) |  | [optional] 
**status** | **String** |  | 
**usage** | [**Usage**](Usage.md) |  | [optional] 



## Enum: ObjectEnum


* `video` (value: `"video"`)





## Enum: StatusEnum


* `pending` (value: `"pending"`)

* `running` (value: `"running"`)

* `succeeded` (value: `"succeeded"`)

* `failed` (value: `"failed"`)

* `cancelled` (value: `"cancelled"`)

* `expired` (value: `"expired"`)




