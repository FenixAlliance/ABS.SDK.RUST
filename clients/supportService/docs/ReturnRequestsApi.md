# \ReturnRequestsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_return_request_async**](ReturnRequestsApi.md#create_return_request_async) | **POST** /api/v2/SupportService/ReturnRequests | Create a return request
[**delete_return_request_async**](ReturnRequestsApi.md#delete_return_request_async) | **DELETE** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Delete a return request
[**get_return_request_async**](ReturnRequestsApi.md#get_return_request_async) | **GET** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Retrieve a return request by ID
[**get_return_requests_async**](ReturnRequestsApi.md#get_return_requests_async) | **GET** /api/v2/SupportService/ReturnRequests | Retrieve return requests
[**get_return_requests_count_async**](ReturnRequestsApi.md#get_return_requests_count_async) | **GET** /api/v2/SupportService/ReturnRequests/Count | Get return requests count
[**update_return_request_async**](ReturnRequestsApi.md#update_return_request_async) | **PUT** /api/v2/SupportService/ReturnRequests/{returnRequestId} | Update a return request



## create_return_request_async

> models::EmptyEnvelope create_return_request_async(tenant_id, api_version, x_api_version, return_request_create_dto)
Create a return request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**return_request_create_dto** | Option<[**ReturnRequestCreateDto**](ReturnRequestCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_return_request_async

> models::EmptyEnvelope delete_return_request_async(tenant_id, return_request_id, api_version, x_api_version)
Delete a return request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_request_id** | **uuid::Uuid** |  | [required] |
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


## get_return_request_async

> models::ReturnRequestDtoEnvelope get_return_request_async(tenant_id, return_request_id, api_version, x_api_version)
Retrieve a return request by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ReturnRequestDtoEnvelope**](ReturnRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_return_requests_async

> models::ReturnRequestDtoListEnvelope get_return_requests_async(tenant_id, api_version, x_api_version)
Retrieve return requests

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ReturnRequestDtoListEnvelope**](ReturnRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_return_requests_count_async

> models::Int32Envelope get_return_requests_count_async(tenant_id, api_version, x_api_version)
Get return requests count

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


## update_return_request_async

> models::EmptyEnvelope update_return_request_async(tenant_id, return_request_id, api_version, x_api_version, return_request_update_dto)
Update a return request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**return_request_update_dto** | Option<[**ReturnRequestUpdateDto**](ReturnRequestUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

