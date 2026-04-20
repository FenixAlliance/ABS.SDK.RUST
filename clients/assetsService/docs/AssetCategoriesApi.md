# \AssetCategoriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_asset_category**](AssetCategoriesApi.md#create_asset_category) | **POST** /api/v2/AssetsService/AssetCategories | Creates a new asset category
[**delete_asset_category**](AssetCategoriesApi.md#delete_asset_category) | **DELETE** /api/v2/AssetsService/AssetCategories/{categoryId} | Deletes an asset category
[**get_asset_categories**](AssetCategoriesApi.md#get_asset_categories) | **GET** /api/v2/AssetsService/AssetCategories | Gets all asset categories for the current tenant
[**get_asset_categories_count**](AssetCategoriesApi.md#get_asset_categories_count) | **GET** /api/v2/AssetsService/AssetCategories/count | Gets the count of asset categories
[**get_asset_category**](AssetCategoriesApi.md#get_asset_category) | **GET** /api/v2/AssetsService/AssetCategories/{categoryId} | Gets a specific asset category
[**update_asset_category**](AssetCategoriesApi.md#update_asset_category) | **PUT** /api/v2/AssetsService/AssetCategories/{categoryId} | Updates an existing asset category



## create_asset_category

> models::AssetCategoryDtoEnvelope create_asset_category(tenant_id, asset_category_create_dto)
Creates a new asset category

Creates a new asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_category_create_dto** | Option<[**AssetCategoryCreateDto**](AssetCategoryCreateDto.md)> |  |  |

### Return type

[**models::AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_category

> delete_asset_category(tenant_id, category_id)
Deletes an asset category

Deletes an asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_categories

> models::AssetCategoryDtoListEnvelope get_asset_categories(tenant_id)
Gets all asset categories for the current tenant

Retrieves all asset categories for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetCategoryDtoListEnvelope**](AssetCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_categories_count

> models::Int32Envelope get_asset_categories_count(tenant_id)
Gets the count of asset categories

Returns the total number of asset categories for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_category

> models::AssetCategoryDtoEnvelope get_asset_category(tenant_id, category_id)
Gets a specific asset category

Retrieves a specific asset category by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_category

> models::EmptyEnvelope update_asset_category(tenant_id, category_id, asset_category_update_dto)
Updates an existing asset category

Updates an existing asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
**asset_category_update_dto** | Option<[**AssetCategoryUpdateDto**](AssetCategoryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

