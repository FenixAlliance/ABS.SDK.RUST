# \ItemGoogleCategoriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_all_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/All | Get all Google item categories (all)
[**get_children_item_google_categories_by_id_async**](ItemGoogleCategoriesApi.md#get_children_item_google_categories_by_id_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/{itemCategoryId}/Children | Get children Google item categories by ID
[**get_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories | Get all Google item categories
[**get_item_google_categories_count_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_count_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/Count | Get Google item categories count
[**get_item_google_categories_tree_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_tree_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/tree | Get Google item categories tree
[**get_item_google_category_by_id_async**](ItemGoogleCategoriesApi.md#get_item_google_category_by_id_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/{itemCategoryId} | Get Google item category by ID
[**get_root_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_root_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/Primary | Get root Google item categories
[**map_item_google_categories_tree_async**](ItemGoogleCategoriesApi.md#map_item_google_categories_tree_async) | **POST** /api/v2/CatalogService/ItemGoogleCategories/tree | Map Google item categories tree



## get_all_item_google_categories_async

> models::ItemGoogleCategoryDtoListEnvelope get_all_item_google_categories_async(api_version, x_api_version)
Get all Google item categories (all)

Retrieves all Google item categories (all) without OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_children_item_google_categories_by_id_async

> models::ItemGoogleCategoryDtoListEnvelope get_children_item_google_categories_by_id_async(item_category_id, api_version, x_api_version)
Get children Google item categories by ID

Retrieves children Google item categories for a given ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_category_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_google_categories_async

> models::ItemGoogleCategoryDtoListEnvelope get_item_google_categories_async(api_version, x_api_version)
Get all Google item categories

Retrieves all Google item categories using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_google_categories_count_async

> models::Int32Envelope get_item_google_categories_count_async(api_version, x_api_version)
Get Google item categories count

Retrieves the count of Google item categories using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_item_google_categories_tree_async

> models::ItemGoogleCategoryDtoListEnvelope get_item_google_categories_tree_async(api_version, x_api_version)
Get Google item categories tree

Retrieves the Google item categories tree.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_google_category_by_id_async

> models::ItemGoogleCategoryDtoEnvelope get_item_google_category_by_id_async(item_category_id, api_version, x_api_version)
Get Google item category by ID

Retrieves a specific Google item category by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_category_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_root_item_google_categories_async

> models::ItemGoogleCategoryDtoListEnvelope get_root_item_google_categories_async(api_version, x_api_version)
Get root Google item categories

Retrieves root Google item categories.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## map_item_google_categories_tree_async

> models::ItemGoogleCategoryDtoListEnvelope map_item_google_categories_tree_async(tenant_id, api_version, x_api_version)
Map Google item categories tree

Maps the Google item categories tree.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

