# \ItemTagsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_tag_async**](ItemTagsApi.md#create_item_tag_async) | **POST** /api/v2/CatalogService/ItemTags | Create a new item tag
[**delete_item_tag_async**](ItemTagsApi.md#delete_item_tag_async) | **DELETE** /api/v2/CatalogService/ItemTags/{itemTagId} | Delete an item tag
[**get_item_tag_by_id_async**](ItemTagsApi.md#get_item_tag_by_id_async) | **GET** /api/v2/CatalogService/ItemTags/{itemTagId} | Get item tag by ID
[**get_item_tags_async**](ItemTagsApi.md#get_item_tags_async) | **GET** /api/v2/CatalogService/ItemTags | Get all item tags
[**update_item_tag_async**](ItemTagsApi.md#update_item_tag_async) | **PUT** /api/v2/CatalogService/ItemTags/{itemTagId} | Update an item tag



## create_item_tag_async

> models::ItemTagDtoEnvelope create_item_tag_async(tenant_id, api_version, x_api_version, item_tag_create_dto)
Create a new item tag

Creates a new item tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_tag_create_dto** | Option<[**ItemTagCreateDto**](ItemTagCreateDto.md)> |  |  |

### Return type

[**models::ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_tag_async

> delete_item_tag_async(tenant_id, item_tag_id, api_version, x_api_version)
Delete an item tag

Deletes an item tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_tag_id** | **uuid::Uuid** |  | [required] |
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


## get_item_tag_by_id_async

> models::ItemTagDtoEnvelope get_item_tag_by_id_async(item_tag_id, api_version, x_api_version)
Get item tag by ID

Retrieves a specific item tag by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_tags_async

> models::ItemTagDtoListEnvelope get_item_tags_async(tenant_id, api_version, x_api_version)
Get all item tags

Retrieves all item tags for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoListEnvelope**](ItemTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_tag_async

> update_item_tag_async(tenant_id, item_tag_id, api_version, x_api_version, item_tag_update_dto)
Update an item tag

Updates an existing item tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_tag_update_dto** | Option<[**ItemTagUpdateDto**](ItemTagUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

