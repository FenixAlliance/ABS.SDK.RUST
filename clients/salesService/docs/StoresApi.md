# \StoresApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_stores_async**](StoresApi.md#count_stores_async) | **GET** /api/v2/SalesService/Stores/Count | Get stores count
[**create_store_async**](StoresApi.md#create_store_async) | **POST** /api/v2/SalesService/Stores | Create a store
[**delete_store_async**](StoresApi.md#delete_store_async) | **DELETE** /api/v2/SalesService/Stores/{storeId} | Delete a store
[**get_store_async**](StoresApi.md#get_store_async) | **GET** /api/v2/SalesService/Stores/{storeId} | Get store by ID
[**get_stores_async**](StoresApi.md#get_stores_async) | **GET** /api/v2/SalesService/Stores | Get stores
[**update_store_async**](StoresApi.md#update_store_async) | **PUT** /api/v2/SalesService/Stores/{storeId} | Update a store



## count_stores_async

> models::Int32Envelope count_stores_async(tenant_id)
Get stores count

Returns the total count of stores for the specified tenant with OData filter support.

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


## create_store_async

> models::EmptyEnvelope create_store_async(tenant_id, store_create_dto)
Create a store

Creates a new store for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**store_create_dto** | Option<[**StoreCreateDto**](StoreCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_store_async

> models::EmptyEnvelope delete_store_async(tenant_id, store_id)
Delete a store

Deletes an existing store by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**store_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_store_async

> models::StoreDtoEnvelope get_store_async(tenant_id, store_id)
Get store by ID

Retrieves a single store by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**store_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::StoreDtoEnvelope**](StoreDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stores_async

> models::StoreDtoListEnvelope get_stores_async(tenant_id)
Get stores

Retrieves a list of stores for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::StoreDtoListEnvelope**](StoreDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_store_async

> models::EmptyEnvelope update_store_async(tenant_id, store_id, store_update_dto)
Update a store

Updates an existing store by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**store_id** | **uuid::Uuid** |  | [required] |
**store_update_dto** | Option<[**StoreUpdateDto**](StoreUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

