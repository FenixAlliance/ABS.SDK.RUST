# \LogsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_logs_async**](LogsApi.md#get_logs_async) | **GET** /api/v2/SecurityService/Logs | Get tenant logs
[**get_logs_count_async**](LogsApi.md#get_logs_count_async) | **GET** /api/v2/SecurityService/Logs/Count | Get tenant logs count



## get_logs_async

> models::LogDtoListEnvelope get_logs_async(tenant_id, api_version, x_api_version, log_dto_collection_query_parameters)
Get tenant logs

Retrieves logs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**log_dto_collection_query_parameters** | Option<[**LogDtoCollectionQueryParameters**](LogDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::LogDtoListEnvelope**](LogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_logs_count_async

> models::Int32Envelope get_logs_count_async(tenant_id, api_version, x_api_version, log_dto_collection_query_parameters)
Get tenant logs count

Retrieves the count of logs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**log_dto_collection_query_parameters** | Option<[**LogDtoCollectionQueryParameters**](LogDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

