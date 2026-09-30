# MmGatewayJs.ImageTaskResponse

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
**object** | **String** |  | [optional] [default to &#39;image&#39;]
**outputs** | [**[ImageOutput]**](ImageOutput.md) |  | [optional] 
**status** | **String** |  | 
**usage** | [**Usage**](Usage.md) |  | [optional] 



## Enum: ObjectEnum


* `image` (value: `"image"`)





## Enum: StatusEnum


* `pending` (value: `"pending"`)

* `running` (value: `"running"`)

* `succeeded` (value: `"succeeded"`)

* `failed` (value: `"failed"`)

* `cancelled` (value: `"cancelled"`)

* `expired` (value: `"expired"`)




