# \SupportRequestAttachmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_request_attachment_async**](SupportRequestAttachmentsApi.md#create_support_request_attachment_async) | **POST** /api/v2/SupportService/SupportRequestAttachments | Create a new support request attachment
[**delete_support_request_attachment_async**](SupportRequestAttachmentsApi.md#delete_support_request_attachment_async) | **DELETE** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Delete a support request attachment
[**get_support_request_attachment_async**](SupportRequestAttachmentsApi.md#get_support_request_attachment_async) | **GET** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Retrieve a support request attachment by ID
[**get_support_request_attachments_async**](SupportRequestAttachmentsApi.md#get_support_request_attachments_async) | **GET** /api/v2/SupportService/SupportRequestAttachments | Retrieve a list of support request attachments
[**get_support_request_attachments_count_async**](SupportRequestAttachmentsApi.md#get_support_request_attachments_count_async) | **GET** /api/v2/SupportService/SupportRequestAttachments/Count | Get the count of support request attachments
[**update_support_request_attachment_async**](SupportRequestAttachmentsApi.md#update_support_request_attachment_async) | **PUT** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Update a support request attachment



## create_support_request_attachment_async

> models::EmptyEnvelope create_support_request_attachment_async(tenant_id, api_version, x_api_version, support_request_attachment_create_dto)
Create a new support request attachment

Creates a new support request attachment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_request_attachment_create_dto** | Option<[**SupportRequestAttachmentCreateDto**](SupportRequestAttachmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_request_attachment_async

> models::EmptyEnvelope delete_support_request_attachment_async(tenant_id, support_request_attachment_id, api_version, x_api_version)
Delete a support request attachment

Deletes a support request attachment by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_attachment_id** | **uuid::Uuid** |  | [required] |
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


## get_support_request_attachment_async

> models::SupportRequestAttachmentDtoEnvelope get_support_request_attachment_async(tenant_id, support_request_attachment_id, api_version, x_api_version)
Retrieve a support request attachment by ID

Retrieves a single support request attachment by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestAttachmentDtoEnvelope**](SupportRequestAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_request_attachments_async

> models::SupportRequestAttachmentDtoListEnvelope get_support_request_attachments_async(tenant_id, api_version, x_api_version)
Retrieve a list of support request attachments

Retrieves a list of support request attachments for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestAttachmentDtoListEnvelope**](SupportRequestAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_request_attachments_count_async

> models::Int32Envelope get_support_request_attachments_count_async(tenant_id, api_version, x_api_version)
Get the count of support request attachments

Returns the total count of support request attachments for the specified tenant with OData query support.

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


## update_support_request_attachment_async

> models::EmptyEnvelope update_support_request_attachment_async(tenant_id, support_request_attachment_id, api_version, x_api_version, support_request_attachment_update_dto)
Update a support request attachment

Updates an existing support request attachment by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_request_attachment_update_dto** | Option<[**SupportRequestAttachmentUpdateDto**](SupportRequestAttachmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

