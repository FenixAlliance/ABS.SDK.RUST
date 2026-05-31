# \ItemFamiliesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_family_async**](ItemFamiliesApi.md#create_item_family_async) | **POST** /api/v2/CatalogService/ItemFamilies | Create a new item family
[**delete_item_family_async**](ItemFamiliesApi.md#delete_item_family_async) | **DELETE** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Delete an item family
[**get_item_families_async**](ItemFamiliesApi.md#get_item_families_async) | **GET** /api/v2/CatalogService/ItemFamilies | Get all item families
[**get_item_families_count_async**](ItemFamiliesApi.md#get_item_families_count_async) | **GET** /api/v2/CatalogService/ItemFamilies/Count | Get item families count
[**get_item_family_by_id_async**](ItemFamiliesApi.md#get_item_family_by_id_async) | **GET** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Get item family by ID
[**update_item_family_async**](ItemFamiliesApi.md#update_item_family_async) | **PUT** /api/v2/CatalogService/ItemFamilies/{itemFamilyId} | Update an item family



## create_item_family_async

> models::ItemFamilyDtoEnvelope create_item_family_async(tenant_id, api_version, x_api_version, item_family_create_dto)
Create a new item family

Creates a new item family for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_family_create_dto** | Option<[**ItemFamilyCreateDto**](ItemFamilyCreateDto.md)> |  |  |

### Return type

[**models::ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_family_async

> delete_item_family_async(tenant_id, item_family_id, api_version, x_api_version)
Delete an item family

Deletes an item family for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_family_id** | **uuid::Uuid** |  | [required] |
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


## get_item_families_async

> models::ItemFamilyDtoListEnvelope get_item_families_async(tenant_id, api_version, x_api_version)
Get all item families

Retrieves all item families for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemFamilyDtoListEnvelope**](ItemFamilyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_families_count_async

> models::Int32Envelope get_item_families_count_async(tenant_id, api_version, x_api_version)
Get item families count

Returns the count of item families for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## get_item_family_by_id_async

> models::ItemFamilyDtoEnvelope get_item_family_by_id_async(item_family_id, tenant_id, api_version, x_api_version)
Get item family by ID

Retrieves a specific item family by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_family_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_family_async

> models::ItemFamilyDtoEnvelope update_item_family_async(tenant_id, item_family_id, api_version, x_api_version, item_family_update_dto)
Update an item family

Updates an existing item family for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_family_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_family_update_dto** | Option<[**ItemFamilyUpdateDto**](ItemFamilyUpdateDto.md)> |  |  |

### Return type

[**models::ItemFamilyDtoEnvelope**](ItemFamilyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

