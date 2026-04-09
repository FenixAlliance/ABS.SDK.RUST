# \ItemCategoriesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_categories_async**](ItemCategoriesApi.md#count_item_categories_async) | **GET** /api/v2/CatalogService/ItemCategories/Count | Count item categories
[**create_item_category_async**](ItemCategoriesApi.md#create_item_category_async) | **POST** /api/v2/CatalogService/ItemCategories | Create a new item category
[**delete_item_category_async**](ItemCategoriesApi.md#delete_item_category_async) | **DELETE** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Delete an item category
[**get_item_categories_async**](ItemCategoriesApi.md#get_item_categories_async) | **GET** /api/v2/CatalogService/ItemCategories | Get all item categories
[**get_item_category_by_id_async**](ItemCategoriesApi.md#get_item_category_by_id_async) | **GET** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Get item category by ID
[**update_item_category_async**](ItemCategoriesApi.md#update_item_category_async) | **PUT** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Update an item category



## count_item_categories_async

> models::Int32Envelope count_item_categories_async(tenant_id, api_version, x_api_version)
Count item categories

Counts all item categories for the specified tenant.

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


## create_item_category_async

> models::ItemCategoryDtoEnvelope create_item_category_async(tenant_id, api_version, x_api_version, item_category_create_dto)
Create a new item category

Creates a new item category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_category_create_dto** | Option<[**ItemCategoryCreateDto**](ItemCategoryCreateDto.md)> |  |  |

### Return type

[**models::ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_category_async

> delete_item_category_async(tenant_id, item_category_id, api_version, x_api_version)
Delete an item category

Deletes an item category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_category_id** | **uuid::Uuid** |  | [required] |
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


## get_item_categories_async

> models::ItemCategoryDtoListEnvelope get_item_categories_async(tenant_id, api_version, x_api_version)
Get all item categories

Retrieves all item categories for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoListEnvelope**](ItemCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_category_by_id_async

> models::ItemCategoryDtoEnvelope get_item_category_by_id_async(item_category_id, api_version, x_api_version)
Get item category by ID

Retrieves a specific item category by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_category_async

> update_item_category_async(tenant_id, item_category_id, api_version, x_api_version, item_category_update_dto)
Update an item category

Updates an existing item category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_category_update_dto** | Option<[**ItemCategoryUpdateDto**](ItemCategoryUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

