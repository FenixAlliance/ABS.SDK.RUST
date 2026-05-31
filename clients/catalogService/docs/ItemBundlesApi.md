# \ItemBundlesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_bundle_async**](ItemBundlesApi.md#create_item_bundle_async) | **POST** /api/v2/CatalogService/ItemBundles | Create a new item bundle
[**delete_item_bundle_async**](ItemBundlesApi.md#delete_item_bundle_async) | **DELETE** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Delete an item bundle
[**get_item_bundle_by_id_async**](ItemBundlesApi.md#get_item_bundle_by_id_async) | **GET** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Get item bundle by ID
[**get_item_bundles_async**](ItemBundlesApi.md#get_item_bundles_async) | **GET** /api/v2/CatalogService/ItemBundles | Get all item bundles
[**get_item_bundles_count_async**](ItemBundlesApi.md#get_item_bundles_count_async) | **GET** /api/v2/CatalogService/ItemBundles/Count | Get item bundles count
[**update_item_bundle_async**](ItemBundlesApi.md#update_item_bundle_async) | **PUT** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Update an item bundle



## create_item_bundle_async

> models::ItemBundleDtoEnvelope create_item_bundle_async(tenant_id, api_version, x_api_version, item_bundle_create_dto)
Create a new item bundle

Creates a new item bundle for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_bundle_create_dto** | Option<[**ItemBundleCreateDto**](ItemBundleCreateDto.md)> |  |  |

### Return type

[**models::ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_bundle_async

> delete_item_bundle_async(tenant_id, item_bundle_id, api_version, x_api_version)
Delete an item bundle

Deletes an item bundle for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_bundle_id** | **uuid::Uuid** |  | [required] |
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


## get_item_bundle_by_id_async

> models::ItemBundleDtoEnvelope get_item_bundle_by_id_async(item_bundle_id, tenant_id, api_version, x_api_version)
Get item bundle by ID

Retrieves a specific item bundle by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_bundle_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_bundles_async

> models::ItemBundleDtoListEnvelope get_item_bundles_async(tenant_id, api_version, x_api_version)
Get all item bundles

Retrieves all item bundles for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBundleDtoListEnvelope**](ItemBundleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_bundles_count_async

> models::Int32Envelope get_item_bundles_count_async(tenant_id, api_version, x_api_version)
Get item bundles count

Returns the count of item bundles for the specified tenant.

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


## update_item_bundle_async

> models::ItemBundleDtoEnvelope update_item_bundle_async(tenant_id, item_bundle_id, api_version, x_api_version, item_bundle_update_dto)
Update an item bundle

Updates an existing item bundle for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_bundle_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_bundle_update_dto** | Option<[**ItemBundleUpdateDto**](ItemBundleUpdateDto.md)> |  |  |

### Return type

[**models::ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

