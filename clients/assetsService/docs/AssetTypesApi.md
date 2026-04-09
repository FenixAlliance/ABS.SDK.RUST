# \AssetTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_asset_type**](AssetTypesApi.md#create_asset_type) | **POST** /api/v2/AssetsService/AssetTypes | Creates a new asset type
[**delete_asset_type**](AssetTypesApi.md#delete_asset_type) | **DELETE** /api/v2/AssetsService/AssetTypes/{typeId} | Deletes an asset type
[**get_asset_type**](AssetTypesApi.md#get_asset_type) | **GET** /api/v2/AssetsService/AssetTypes/{typeId} | Gets a specific asset type
[**get_asset_types**](AssetTypesApi.md#get_asset_types) | **GET** /api/v2/AssetsService/AssetTypes | Gets all asset types for the current tenant
[**get_asset_types_count**](AssetTypesApi.md#get_asset_types_count) | **GET** /api/v2/AssetsService/AssetTypes/count | Gets the count of asset types
[**update_asset_type**](AssetTypesApi.md#update_asset_type) | **PUT** /api/v2/AssetsService/AssetTypes/{typeId} | Updates an existing asset type



## create_asset_type

> models::AssetTypeDtoEnvelope create_asset_type(tenant_id, asset_type_create_dto)
Creates a new asset type

Creates a new asset type for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_type_create_dto** | Option<[**AssetTypeCreateDto**](AssetTypeCreateDto.md)> |  |  |

### Return type

[**models::AssetTypeDtoEnvelope**](AssetTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_type

> delete_asset_type(tenant_id, type_id)
Deletes an asset type

Deletes an asset type for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**type_id** | **uuid::Uuid** |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_type

> models::AssetTypeDtoEnvelope get_asset_type(tenant_id, type_id)
Gets a specific asset type

Retrieves a specific asset type by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**type_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTypeDtoEnvelope**](AssetTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_types

> models::AssetTypeDtoListEnvelope get_asset_types(tenant_id)
Gets all asset types for the current tenant

Retrieves all asset types for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTypeDtoListEnvelope**](AssetTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_types_count

> models::Int32Envelope get_asset_types_count(tenant_id)
Gets the count of asset types

Returns the total number of asset types for the authenticated tenant.

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


## update_asset_type

> models::EmptyEnvelope update_asset_type(tenant_id, type_id, asset_type_update_dto)
Updates an existing asset type

Updates an existing asset type for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**type_id** | **uuid::Uuid** |  | [required] |
**asset_type_update_dto** | Option<[**AssetTypeUpdateDto**](AssetTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

