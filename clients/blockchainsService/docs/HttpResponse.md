# HttpResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_context** | Option<[**models::HttpContext**](HttpContext.md)> |  | [optional]
**status_code** | Option<**i32**> |  | [optional]
**headers** | Option<[**std::collections::HashMap<String, Vec<String>>**](Vec.md)> |  | [optional][readonly]
**body** | Option<[**std::path::PathBuf**](std::path::PathBuf.md)> |  | [optional]
**body_writer** | Option<[**models::PipeWriter**](PipeWriter.md)> |  | [optional]
**content_length** | Option<**i64**> |  | [optional]
**content_type** | Option<**String**> |  | [optional]
**cookies** | Option<[**serde_json::Value**](.md)> |  | [optional]
**has_started** | Option<**bool**> |  | [optional][readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


