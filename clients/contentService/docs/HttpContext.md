# HttpContext

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**features** | Option<[**Vec<models::TypeObjectKeyValuePair>**](TypeObjectKeyValuePair.md)> |  | [optional][readonly]
**request** | Option<[**models::HttpRequest**](HttpRequest.md)> |  | [optional]
**response** | Option<[**models::HttpResponse**](HttpResponse.md)> |  | [optional]
**connection** | Option<[**models::ConnectionInfo**](ConnectionInfo.md)> |  | [optional]
**web_sockets** | Option<[**models::WebSocketManager**](WebSocketManager.md)> |  | [optional]
**user** | Option<[**models::ClaimsPrincipal**](ClaimsPrincipal.md)> |  | [optional]
**items** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> |  | [optional]
**request_services** | Option<[**serde_json::Value**](.md)> |  | [optional]
**request_aborted** | Option<[**models::CancellationToken**](CancellationToken.md)> |  | [optional]
**trace_identifier** | Option<**String**> |  | [optional]
**session** | Option<[**models::ISession**](ISession.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


