# \SignedDocumentAttachmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#create_signed_document_attachment_async) | **POST** /api/v2/TrustService/SignedDocumentAttachments | Create a new signed document attachment
[**delete_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#delete_signed_document_attachment_async) | **DELETE** /api/v2/TrustService/SignedDocumentAttachments/{id} | Delete a signed document attachment
[**get_signed_document_attachment_by_id_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachment_by_id_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments/{id} | Get signed document attachment by ID
[**get_signed_document_attachments_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachments_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments | Get all signed document attachments
[**get_signed_document_attachments_count_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachments_count_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments/Count | Get signed document attachments count
[**patch_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#patch_signed_document_attachment_async) | **PATCH** /api/v2/TrustService/SignedDocumentAttachments/{id} | Patch a signed document attachment
[**update_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#update_signed_document_attachment_async) | **PUT** /api/v2/TrustService/SignedDocumentAttachments/{id} | Update a signed document attachment



## create_signed_document_attachment_async

> create_signed_document_attachment_async(tenant_id, api_version, x_api_version, signed_document_attachment_create_dto)
Create a new signed document attachment

Links an already-stored file to a SignedDocument (metadata + Storage pointer; no bytes).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signed_document_attachment_create_dto** | Option<[**SignedDocumentAttachmentCreateDto**](SignedDocumentAttachmentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_signed_document_attachment_async

> delete_signed_document_attachment_async(tenant_id, id, api_version, x_api_version)
Delete a signed document attachment

Deletes a signed document attachment link for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signed_document_attachment_by_id_async

> models::SignedDocumentAttachmentDto get_signed_document_attachment_by_id_async(tenant_id, id, api_version, x_api_version)
Get signed document attachment by ID

Retrieves a specific signed document attachment by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignedDocumentAttachmentDto**](SignedDocumentAttachmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signed_document_attachments_async

> models::SignedDocumentAttachmentDtoListEnvelope get_signed_document_attachments_async(tenant_id, api_version, x_api_version)
Get all signed document attachments

Retrieves all signed document attachments for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignedDocumentAttachmentDtoListEnvelope**](SignedDocumentAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signed_document_attachments_count_async

> models::Int32Envelope get_signed_document_attachments_count_async(tenant_id, api_version, x_api_version)
Get signed document attachments count

Returns the count of signed document attachments for the specified tenant.

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


## patch_signed_document_attachment_async

> models::EmptyEnvelope patch_signed_document_attachment_async(tenant_id, id, api_version, x_api_version, operation)
Patch a signed document attachment

Patch a signed document attachment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_signed_document_attachment_async

> update_signed_document_attachment_async(tenant_id, id, api_version, x_api_version, signed_document_attachment_update_dto)
Update a signed document attachment

Updates signed document attachment metadata for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signed_document_attachment_update_dto** | Option<[**SignedDocumentAttachmentUpdateDto**](SignedDocumentAttachmentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

