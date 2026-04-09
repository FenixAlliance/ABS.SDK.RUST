# \SizesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_size**](SizesApi.md#create_tenant_size) | **POST** /api/v2/TenantsService/Sizes | Create a new tenant size
[**delete_tenant_size**](SizesApi.md#delete_tenant_size) | **DELETE** /api/v2/TenantsService/Sizes/{tenantSizeId} | Delete a tenant size
[**get_tenant_size_by_id**](SizesApi.md#get_tenant_size_by_id) | **GET** /api/v2/TenantsService/Sizes/{tenantSizeId} | Retrieve a single tenant size by its ID
[**get_tenant_sizes**](SizesApi.md#get_tenant_sizes) | **GET** /api/v2/TenantsService/Sizes | Retrieve a list of tenant sizes
[**get_tenant_sizes_count**](SizesApi.md#get_tenant_sizes_count) | **GET** /api/v2/TenantsService/Sizes/Count | Get the count of tenant sizes
[**update_tenant_size**](SizesApi.md#update_tenant_size) | **PUT** /api/v2/TenantsService/Sizes/{tenantSizeId} | Update a tenant size



## create_tenant_size

> models::EmptyEnvelope create_tenant_size(tenant_id, api_version, x_api_version, tenant_size_create_dto)
Create a new tenant size

Create a new tenant size

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_size_create_dto** | Option<[**TenantSizeCreateDto**](TenantSizeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_size

> models::EmptyEnvelope delete_tenant_size(tenant_id, tenant_size_id, api_version, x_api_version)
Delete a tenant size

Delete a tenant size

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_size_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_size_by_id

> models::TenantSizeDtoEnvelope get_tenant_size_by_id(tenant_id, tenant_size_id, api_version, x_api_version)
Retrieve a single tenant size by its ID

Retrieve a single tenant size by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_size_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantSizeDtoEnvelope**](TenantSizeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_sizes

> models::TenantSizeDtoListEnvelope get_tenant_sizes(tenant_id, api_version, x_api_version)
Retrieve a list of tenant sizes

Retrieve a list of tenant sizes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantSizeDtoListEnvelope**](TenantSizeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_sizes_count

> models::Int32Envelope get_tenant_sizes_count(tenant_id, api_version, x_api_version)
Get the count of tenant sizes

Get the count of tenant sizes

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


## update_tenant_size

> models::EmptyEnvelope update_tenant_size(tenant_id, tenant_size_id, api_version, x_api_version, tenant_size_update_dto)
Update a tenant size

Update a tenant size

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_size_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_size_update_dto** | Option<[**TenantSizeUpdateDto**](TenantSizeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

