# \ItemBrandsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_brand_async**](ItemBrandsApi.md#create_item_brand_async) | **POST** /api/v2/CatalogService/ItemBrands | Create a new item brand
[**delete_item_brand_async**](ItemBrandsApi.md#delete_item_brand_async) | **DELETE** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Delete an item brand
[**get_item_brand_by_id_async**](ItemBrandsApi.md#get_item_brand_by_id_async) | **GET** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Get item brand by ID
[**get_item_brands_async**](ItemBrandsApi.md#get_item_brands_async) | **GET** /api/v2/CatalogService/ItemBrands | Get all item brands
[**update_item_brand_async**](ItemBrandsApi.md#update_item_brand_async) | **PUT** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Update an item brand



## create_item_brand_async

> models::ItemBrandDtoEnvelope create_item_brand_async(tenant_id, api_version, x_api_version, item_brand_create_dto)
Create a new item brand

Creates a new item brand for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_brand_create_dto** | Option<[**ItemBrandCreateDto**](ItemBrandCreateDto.md)> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_brand_async

> delete_item_brand_async(tenant_id, item_brand_id, api_version, x_api_version)
Delete an item brand

Deletes an item brand for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_brand_id** | **uuid::Uuid** |  | [required] |
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


## get_item_brand_by_id_async

> models::ItemBrandDtoEnvelope get_item_brand_by_id_async(item_brand_id, api_version, x_api_version)
Get item brand by ID

Retrieves a specific item brand by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_brand_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_brands_async

> models::ItemBrandDtoListEnvelope get_item_brands_async(tenant_id, api_version, x_api_version)
Get all item brands

Retrieves all item brands for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoListEnvelope**](ItemBrandDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_brand_async

> models::ItemBrandDtoEnvelope update_item_brand_async(tenant_id, item_brand_id, api_version, x_api_version, item_brand_update_dto)
Update an item brand

Updates an existing item brand for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_brand_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_brand_update_dto** | Option<[**ItemBrandUpdateDto**](ItemBrandUpdateDto.md)> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

