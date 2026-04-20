# \TypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_type**](TypesApi.md#create_tenant_type) | **POST** /api/v2/TenantsService/Types | Create a new tenant type
[**delete_tenant_type**](TypesApi.md#delete_tenant_type) | **DELETE** /api/v2/TenantsService/Types/{tenantTypeId} | Delete a tenant type
[**get_tenant_type_by_id**](TypesApi.md#get_tenant_type_by_id) | **GET** /api/v2/TenantsService/Types/{tenantTypeId} | Retrieve a single tenant type by its ID
[**get_tenant_types**](TypesApi.md#get_tenant_types) | **GET** /api/v2/TenantsService/Types | Retrieve a list of tenant types
[**get_tenant_types_count**](TypesApi.md#get_tenant_types_count) | **GET** /api/v2/TenantsService/Types/Count | Get the count of tenant types
[**update_tenant_type**](TypesApi.md#update_tenant_type) | **PUT** /api/v2/TenantsService/Types/{tenantTypeId} | Update a tenant type



## create_tenant_type

> models::EmptyEnvelope create_tenant_type(tenant_id, api_version, x_api_version, tenant_type_create_dto)
Create a new tenant type

Create a new tenant type

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_type_create_dto** | Option<[**TenantTypeCreateDto**](TenantTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_type

> models::EmptyEnvelope delete_tenant_type(tenant_id, tenant_type_id, api_version, x_api_version)
Delete a tenant type

Delete a tenant type

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_type_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_type_by_id

> models::TenantTypeDtoEnvelope get_tenant_type_by_id(tenant_id, tenant_type_id, api_version, x_api_version)
Retrieve a single tenant type by its ID

Retrieve a single tenant type by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTypeDtoEnvelope**](TenantTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_types

> models::TenantTypeDtoListEnvelope get_tenant_types(tenant_id, api_version, x_api_version)
Retrieve a list of tenant types

Retrieve a list of tenant types

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTypeDtoListEnvelope**](TenantTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_types_count

> models::Int32Envelope get_tenant_types_count(tenant_id, api_version, x_api_version)
Get the count of tenant types

Get the count of tenant types

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


## update_tenant_type

> models::EmptyEnvelope update_tenant_type(tenant_id, tenant_type_id, api_version, x_api_version, tenant_type_update_dto)
Update a tenant type

Update a tenant type

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_type_update_dto** | Option<[**TenantTypeUpdateDto**](TenantTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

