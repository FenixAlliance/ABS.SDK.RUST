# \InquiryRequestsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_inquiry_request_async**](InquiryRequestsApi.md#create_inquiry_request_async) | **POST** /api/v2/SupportService/InquiryRequests | Create an inquiry request
[**delete_inquiry_request_async**](InquiryRequestsApi.md#delete_inquiry_request_async) | **DELETE** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Delete an inquiry request
[**get_inquiry_request_async**](InquiryRequestsApi.md#get_inquiry_request_async) | **GET** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Retrieve an inquiry request by ID
[**get_inquiry_requests_async**](InquiryRequestsApi.md#get_inquiry_requests_async) | **GET** /api/v2/SupportService/InquiryRequests | Retrieve inquiry requests
[**get_inquiry_requests_count_async**](InquiryRequestsApi.md#get_inquiry_requests_count_async) | **GET** /api/v2/SupportService/InquiryRequests/Count | Get inquiry requests count
[**update_inquiry_request_async**](InquiryRequestsApi.md#update_inquiry_request_async) | **PUT** /api/v2/SupportService/InquiryRequests/{inquiryRequestId} | Update an inquiry request



## create_inquiry_request_async

> models::EmptyEnvelope create_inquiry_request_async(tenant_id, api_version, x_api_version, inquiry_request_create_dto)
Create an inquiry request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inquiry_request_create_dto** | Option<[**InquiryRequestCreateDto**](InquiryRequestCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_inquiry_request_async

> models::EmptyEnvelope delete_inquiry_request_async(tenant_id, inquiry_request_id, api_version, x_api_version)
Delete an inquiry request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**inquiry_request_id** | **uuid::Uuid** |  | [required] |
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


## get_inquiry_request_async

> models::InquiryRequestDtoEnvelope get_inquiry_request_async(tenant_id, inquiry_request_id, api_version, x_api_version)
Retrieve an inquiry request by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**inquiry_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InquiryRequestDtoEnvelope**](InquiryRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inquiry_requests_async

> models::InquiryRequestDtoListEnvelope get_inquiry_requests_async(tenant_id, api_version, x_api_version)
Retrieve inquiry requests

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InquiryRequestDtoListEnvelope**](InquiryRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inquiry_requests_count_async

> models::Int32Envelope get_inquiry_requests_count_async(tenant_id, api_version, x_api_version)
Get inquiry requests count

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


## update_inquiry_request_async

> models::EmptyEnvelope update_inquiry_request_async(tenant_id, inquiry_request_id, api_version, x_api_version, inquiry_request_update_dto)
Update an inquiry request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**inquiry_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inquiry_request_update_dto** | Option<[**InquiryRequestUpdateDto**](InquiryRequestUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

