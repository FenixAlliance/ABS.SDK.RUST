# \PostingExecutionsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_posting_executions_async**](PostingExecutionsApi.md#count_posting_executions_async) | **GET** /api/v2/AccountingService/PostingExecutions/Count | Count posting executions
[**get_posting_executions_async**](PostingExecutionsApi.md#get_posting_executions_async) | **GET** /api/v2/AccountingService/PostingExecutions | List posting executions



## count_posting_executions_async

> models::Int32Envelope count_posting_executions_async(tenant_id, api_version, x_api_version, posting_execution_dto_collection_query_parameters)
Count posting executions

Returns the count of the tenant's posting-inbox executions under the same OData shaping as the list read (e.g. $filter=Status eq 'Rejected' to count rejected intents). Requires journals_read.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**posting_execution_dto_collection_query_parameters** | Option<[**PostingExecutionDtoCollectionQueryParameters**](PostingExecutionDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_posting_executions_async

> models::PostingExecutionDtoIReadOnlyListEnvelope get_posting_executions_async(tenant_id, api_version, x_api_version, posting_execution_dto_collection_query_parameters)
List posting executions

Lists the tenant's posting-inbox executions (the durable evidence of every posting intent). Use OData to scope to a state — e.g. $filter=Status eq 'Rejected' for rejected intents, or Status eq 'PendingMapping'/'PendingPeriod'/'PendingRate' for the retryable pending set — and to page/order. Requires journals_read.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**posting_execution_dto_collection_query_parameters** | Option<[**PostingExecutionDtoCollectionQueryParameters**](PostingExecutionDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::PostingExecutionDtoIReadOnlyListEnvelope**](PostingExecutionDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

