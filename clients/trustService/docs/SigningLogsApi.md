# \SigningLogsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_signing_log_by_id_async**](SigningLogsApi.md#get_signing_log_by_id_async) | **GET** /api/v2/TrustService/SigningLogs/{id} | Get signing log by ID
[**get_signing_logs_async**](SigningLogsApi.md#get_signing_logs_async) | **GET** /api/v2/TrustService/SigningLogs | Get all signing logs
[**get_signing_logs_count_async**](SigningLogsApi.md#get_signing_logs_count_async) | **GET** /api/v2/TrustService/SigningLogs/Count | Get signing logs count



## get_signing_log_by_id_async

> models::SigningLogDto get_signing_log_by_id_async(tenant_id, id, api_version, x_api_version)
Get signing log by ID

Retrieves a specific signing log by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningLogDto**](SigningLogDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_logs_async

> models::SigningLogDtoListEnvelope get_signing_logs_async(tenant_id, api_version, x_api_version, signing_log_dto_collection_query_parameters)
Get all signing logs

Retrieves all signing logs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_log_dto_collection_query_parameters** | Option<[**SigningLogDtoCollectionQueryParameters**](SigningLogDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::SigningLogDtoListEnvelope**](SigningLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_logs_count_async

> models::Int32Envelope get_signing_logs_count_async(tenant_id, api_version, x_api_version, signing_log_dto_collection_query_parameters)
Get signing logs count

Returns the count of signing logs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_log_dto_collection_query_parameters** | Option<[**SigningLogDtoCollectionQueryParameters**](SigningLogDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

