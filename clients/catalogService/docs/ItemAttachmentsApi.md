# \ItemAttachmentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_attachment_async**](ItemAttachmentsApi.md#create_item_attachment_async) | **POST** /api/v2/CatalogService/ItemAttachments | Create a new item attachment
[**delete_item_attachment_async**](ItemAttachmentsApi.md#delete_item_attachment_async) | **DELETE** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Delete an item attachment
[**get_item_attachment_by_id_async**](ItemAttachmentsApi.md#get_item_attachment_by_id_async) | **GET** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Get item attachment by ID
[**get_item_attachments_async**](ItemAttachmentsApi.md#get_item_attachments_async) | **GET** /api/v2/CatalogService/ItemAttachments | Get all item attachments
[**update_item_attachment_async**](ItemAttachmentsApi.md#update_item_attachment_async) | **PUT** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Update an item attachment



## create_item_attachment_async

> models::ItemAttachmentDtoEnvelope create_item_attachment_async(tenant_id, api_version, x_api_version, item_attachment_create_dto)
Create a new item attachment

Creates a new item attachment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attachment_create_dto** | Option<[**ItemAttachmentCreateDto**](ItemAttachmentCreateDto.md)> |  |  |

### Return type

[**models::ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_attachment_async

> models::EmptyEnvelope delete_item_attachment_async(tenant_id, item_attachment_id, api_version, x_api_version)
Delete an item attachment

Deletes an item attachment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attachment_id** | **uuid::Uuid** |  | [required] |
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


## get_item_attachment_by_id_async

> models::ItemAttachmentDtoEnvelope get_item_attachment_by_id_async(item_attachment_id, api_version, x_api_version)
Get item attachment by ID

Retrieves a specific item attachment by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_attachments_async

> models::ItemAttachmentDtoListEnvelope get_item_attachments_async(tenant_id, api_version, x_api_version)
Get all item attachments

Retrieves all item attachments for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttachmentDtoListEnvelope**](ItemAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_attachment_async

> models::EmptyEnvelope update_item_attachment_async(tenant_id, item_attachment_id, api_version, x_api_version, item_attachment_update_dto)
Update an item attachment

Updates an existing item attachment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attachment_update_dto** | Option<[**ItemAttachmentUpdateDto**](ItemAttachmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

