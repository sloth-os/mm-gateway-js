# MmGatewayJs.MusicTaskResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**completedAt** | **Date** |  | [optional] 
**createdAt** | **Date** |  | 
**error** | [**TaskError**](TaskError.md) |  | [optional] 
**id** | **String** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | 
**lyrics** | **String** |  | [optional] 
**metadata** | **{String: Object}** |  | [optional] 
**model** | **String** |  | 
**object** | **String** |  | [optional] [default to &#39;music&#39;]
**outputs** | [**[MusicOutput]**](MusicOutput.md) |  | [optional] 
**status** | **String** |  | 
**usage** | [**Usage**](Usage.md) |  | [optional] 



## Enum: ObjectEnum


* `music` (value: `"music"`)





## Enum: StatusEnum


* `pending` (value: `"pending"`)

* `running` (value: `"running"`)

* `succeeded` (value: `"succeeded"`)

* `failed` (value: `"failed"`)

* `cancelled` (value: `"cancelled"`)

* `expired` (value: `"expired"`)




