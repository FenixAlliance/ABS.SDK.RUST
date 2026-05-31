# \RefundRequestsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_refund_request_async**](RefundRequestsApi.md#create_refund_request_async) | **POST** /api/v2/SupportService/RefundRequests | Create a refund request
[**delete_refund_request_async**](RefundRequestsApi.md#delete_refund_request_async) | **DELETE** /api/v2/SupportService/RefundRequests/{refundRequestId} | Delete a refund request
[**get_refund_request_async**](RefundRequestsApi.md#get_refund_request_async) | **GET** /api/v2/SupportService/RefundRequests/{refundRequestId} | Retrieve a refund request by ID
[**get_refund_requests_async**](RefundRequestsApi.md#get_refund_requests_async) | **GET** /api/v2/SupportService/RefundRequests | Retrieve refund requests
[**get_refund_requests_count_async**](RefundRequestsApi.md#get_refund_requests_count_async) | **GET** /api/v2/SupportService/RefundRequests/Count | Get refund requests count
[**update_refund_request_async**](RefundRequestsApi.md#update_refund_request_async) | **PUT** /api/v2/SupportService/RefundRequests/{refundRequestId} | Update a refund request



## create_refund_request_async

> models::EmptyEnvelope create_refund_request_async(tenant_id, api_version, x_api_version, refund_request_create_dto)
Create a refund request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**refund_request_create_dto** | Option<[**RefundRequestCreateDto**](RefundRequestCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_refund_request_async

> models::EmptyEnvelope delete_refund_request_async(tenant_id, refund_request_id, api_version, x_api_version)
Delete a refund request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_refund_request_async

> models::RefundRequestDtoEnvelope get_refund_request_async(tenant_id, refund_request_id, api_version, x_api_version)
Retrieve a refund request by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RefundRequestDtoEnvelope**](RefundRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_refund_requests_async

> models::RefundRequestDtoListEnvelope get_refund_requests_async(tenant_id, api_version, x_api_version)
Retrieve refund requests

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RefundRequestDtoListEnvelope**](RefundRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_refund_requests_count_async

> models::Int32Envelope get_refund_requests_count_async(tenant_id, api_version, x_api_version)
Get refund requests count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_refund_request_async

> models::EmptyEnvelope update_refund_request_async(tenant_id, refund_request_id, api_version, x_api_version, refund_request_update_dto)
Update a refund request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**refund_request_update_dto** | Option<[**RefundRequestUpdateDto**](RefundRequestUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

