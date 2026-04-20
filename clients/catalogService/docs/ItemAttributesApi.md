# \ItemAttributesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_attributes_async**](ItemAttributesApi.md#count_item_attributes_async) | **GET** /api/v2/CatalogService/ItemAttributes/Count | Count item attributes
[**create_item_attribute_async**](ItemAttributesApi.md#create_item_attribute_async) | **POST** /api/v2/CatalogService/ItemAttributes | Create a new item attribute
[**delete_item_attribute_async**](ItemAttributesApi.md#delete_item_attribute_async) | **DELETE** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Delete an item attribute
[**get_item_attribute_by_id_async**](ItemAttributesApi.md#get_item_attribute_by_id_async) | **GET** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Get item attribute by ID
[**get_item_attributes_async**](ItemAttributesApi.md#get_item_attributes_async) | **GET** /api/v2/CatalogService/ItemAttributes | Get all item attributes
[**update_item_attribute_async**](ItemAttributesApi.md#update_item_attribute_async) | **PUT** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Update an item attribute



## count_item_attributes_async

> models::Int32Envelope count_item_attributes_async(tenant_id, api_version, x_api_version)
Count item attributes

Counts all item attributes for the specified tenant.

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


## create_item_attribute_async

> models::ItemAttributeDtoEnvelope create_item_attribute_async(tenant_id, api_version, x_api_version, item_attribute_create_dto)
Create a new item attribute

Creates a new item attribute for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attribute_create_dto** | Option<[**ItemAttributeCreateDto**](ItemAttributeCreateDto.md)> |  |  |

### Return type

[**models::ItemAttributeDtoEnvelope**](ItemAttributeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_attribute_async

> delete_item_attribute_async(tenant_id, item_attribute_id, api_version, x_api_version)
Delete an item attribute

Deletes an item attribute for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attribute_id** | **uuid::Uuid** |  | [required] |
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


## get_item_attribute_by_id_async

> models::ItemAttributeDtoEnvelope get_item_attribute_by_id_async(item_attribute_id, api_version, x_api_version)
Get item attribute by ID

Retrieves a specific item attribute by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_attribute_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeDtoEnvelope**](ItemAttributeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_attributes_async

> models::ItemAttributeDtoListEnvelope get_item_attributes_async(tenant_id, api_version, x_api_version)
Get all item attributes

Retrieves all item attributes for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeDtoListEnvelope**](ItemAttributeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_attribute_async

> update_item_attribute_async(tenant_id, item_attribute_id, api_version, x_api_version, item_attribute_update_dto)
Update an item attribute

Updates an existing item attribute for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attribute_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attribute_update_dto** | Option<[**ItemAttributeUpdateDto**](ItemAttributeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

