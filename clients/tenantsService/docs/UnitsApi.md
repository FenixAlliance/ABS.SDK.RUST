# \UnitsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_unit**](UnitsApi.md#create_tenant_unit) | **POST** /api/v2/TenantsService/Units | Create a new tenant unit
[**delete_tenant_unit**](UnitsApi.md#delete_tenant_unit) | **DELETE** /api/v2/TenantsService/Units/{tenantUnitId} | Delete a tenant unit
[**get_tenant_unit_by_id**](UnitsApi.md#get_tenant_unit_by_id) | **GET** /api/v2/TenantsService/Units/{tenantUnitId} | Retrieve a single tenant unit by its ID
[**get_tenant_units**](UnitsApi.md#get_tenant_units) | **GET** /api/v2/TenantsService/Units | Retrieve a list of tenant units
[**get_tenant_units_count**](UnitsApi.md#get_tenant_units_count) | **GET** /api/v2/TenantsService/Units/Count | Get the count of tenant units
[**update_tenant_unit**](UnitsApi.md#update_tenant_unit) | **PUT** /api/v2/TenantsService/Units/{tenantUnitId} | Update a tenant unit



## create_tenant_unit

> models::EmptyEnvelope create_tenant_unit(tenant_id, api_version, x_api_version, tenant_unit_create_dto)
Create a new tenant unit

Create a new tenant unit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_unit_create_dto** | Option<[**TenantUnitCreateDto**](TenantUnitCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_unit

> models::EmptyEnvelope delete_tenant_unit(tenant_id, tenant_unit_id, api_version, x_api_version)
Delete a tenant unit

Delete a tenant unit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_unit_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_unit_by_id

> models::TenantUnitDtoEnvelope get_tenant_unit_by_id(tenant_id, tenant_unit_id, api_version, x_api_version)
Retrieve a single tenant unit by its ID

Retrieve a single tenant unit by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_unit_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantUnitDtoEnvelope**](TenantUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_units

> models::TenantUnitDtoListEnvelope get_tenant_units(tenant_id, api_version, x_api_version)
Retrieve a list of tenant units

Retrieve a list of tenant units

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantUnitDtoListEnvelope**](TenantUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_units_count

> models::Int32Envelope get_tenant_units_count(tenant_id, api_version, x_api_version)
Get the count of tenant units

Get the count of tenant units

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


## update_tenant_unit

> models::EmptyEnvelope update_tenant_unit(tenant_id, tenant_unit_id, api_version, x_api_version, tenant_unit_update_dto)
Update a tenant unit

Update a tenant unit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_unit_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_unit_update_dto** | Option<[**TenantUnitUpdateDto**](TenantUnitUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

