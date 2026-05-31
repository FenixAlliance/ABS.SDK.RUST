# HttpRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_context** | Option<[**models::HttpContext**](HttpContext.md)> |  | [optional]
**method** | Option<**String**> |  | [optional]
**scheme** | Option<**String**> |  | [optional]
**is_https** | Option<**bool**> |  | [optional]
**host** | Option<[**models::HostString**](HostString.md)> |  | [optional]
**path_base** | Option<[**models::PathString**](PathString.md)> |  | [optional]
**path** | Option<[**models::PathString**](PathString.md)> |  | [optional]
**query_string** | Option<[**models::QueryString**](QueryString.md)> |  | [optional]
**query** | Option<[**Vec<models::StringStringValuesKeyValuePair>**](StringStringValuesKeyValuePair.md)> |  | [optional]
**protocol** | Option<**String**> |  | [optional]
**headers** | Option<[**std::collections::HashMap<String, Vec<String>>**](Vec.md)> |  | [optional][readonly]
**cookies** | Option<[**Vec<models::StringStringKeyValuePair>**](StringStringKeyValuePair.md)> |  | [optional]
**content_length** | Option<**i64**> |  | [optional]
**content_type** | Option<**String**> |  | [optional]
**body** | Option<[**std::path::PathBuf**](std::path::PathBuf.md)> |  | [optional]
**body_reader** | Option<[**std::path::PathBuf**](std::path::PathBuf.md)> |  | [optional][readonly]
**has_form_content_type** | Option<**bool**> |  | [optional][readonly]
**form** | Option<[**Vec<models::StringStringValuesKeyValuePair>**](StringStringValuesKeyValuePair.md)> |  | [optional]
**route_values** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


