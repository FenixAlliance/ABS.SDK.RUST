# \ItemTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_types_async**](ItemTypesApi.md#count_item_types_async) | **GET** /api/v2/CatalogService/ItemTypes/Count | Count item types
[**create_item_type_async**](ItemTypesApi.md#create_item_type_async) | **POST** /api/v2/CatalogService/ItemTypes | Create a new item type
[**delete_item_type_async**](ItemTypesApi.md#delete_item_type_async) | **DELETE** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Delete an item type
[**get_item_type_by_id_async**](ItemTypesApi.md#get_item_type_by_id_async) | **GET** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Get item type by ID
[**get_item_types_async**](ItemTypesApi.md#get_item_types_async) | **GET** /api/v2/CatalogService/ItemTypes | Get all item types
[**update_item_type_async**](ItemTypesApi.md#update_item_type_async) | **PUT** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Update an item type



## count_item_types_async

> models::Int32Envelope count_item_types_async(tenant_id, api_version, x_api_version)
Count item types

Counts all item types for the specified tenant.

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


## create_item_type_async

> models::ItemTypeDtoEnvelope create_item_type_async(tenant_id, api_version, x_api_version, item_type_create_dto)
Create a new item type

Creates a new item type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_type_create_dto** | Option<[**ItemTypeCreateDto**](ItemTypeCreateDto.md)> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_type_async

> models::ItemTypeDtoEnvelope delete_item_type_async(tenant_id, item_type_id, api_version, x_api_version)
Delete an item type

Deletes an item type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_type_by_id_async

> models::ItemTypeDtoEnvelope get_item_type_by_id_async(item_type_id, api_version, x_api_version)
Get item type by ID

Retrieves a specific item type by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_types_async

> models::ItemTypeDtoListEnvelope get_item_types_async(tenant_id, api_version, x_api_version)
Get all item types

Retrieves all item types for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoListEnvelope**](ItemTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_type_async

> update_item_type_async(tenant_id, item_type_id, api_version, x_api_version, item_type_update_dto)
Update an item type

Updates an existing item type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_type_update_dto** | Option<[**ItemTypeUpdateDto**](ItemTypeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

