# \TerritoriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_territory**](TerritoriesApi.md#create_tenant_territory) | **POST** /api/v2/TenantsService/Territories | Create a new tenant territory
[**delete_tenant_territory**](TerritoriesApi.md#delete_tenant_territory) | **DELETE** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Delete a tenant territory
[**get_tenant_territories**](TerritoriesApi.md#get_tenant_territories) | **GET** /api/v2/TenantsService/Territories | Retrieve a list of tenant territories
[**get_tenant_territories_count**](TerritoriesApi.md#get_tenant_territories_count) | **GET** /api/v2/TenantsService/Territories/Count | Get the count of tenant territories
[**get_tenant_territory_by_id**](TerritoriesApi.md#get_tenant_territory_by_id) | **GET** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Retrieve a single tenant territory by its ID
[**update_tenant_territory**](TerritoriesApi.md#update_tenant_territory) | **PUT** /api/v2/TenantsService/Territories/{tenantTerritoryId} | Update a tenant territory



## create_tenant_territory

> models::EmptyEnvelope create_tenant_territory(tenant_id, api_version, x_api_version, tenant_territory_create_dto)
Create a new tenant territory

Create a new tenant territory

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_territory_create_dto** | Option<[**TenantTerritoryCreateDto**](TenantTerritoryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_territory

> models::EmptyEnvelope delete_tenant_territory(tenant_id, tenant_territory_id, api_version, x_api_version)
Delete a tenant territory

Delete a tenant territory

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_territory_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_territories

> models::TenantTerritoryDtoListEnvelope get_tenant_territories(tenant_id, api_version, x_api_version)
Retrieve a list of tenant territories

Retrieve a list of tenant territories

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTerritoryDtoListEnvelope**](TenantTerritoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_territories_count

> models::Int32Envelope get_tenant_territories_count(tenant_id, api_version, x_api_version)
Get the count of tenant territories

Get the count of tenant territories

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


## get_tenant_territory_by_id

> models::TenantTerritoryDtoEnvelope get_tenant_territory_by_id(tenant_id, tenant_territory_id, api_version, x_api_version)
Retrieve a single tenant territory by its ID

Retrieve a single tenant territory by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_territory_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTerritoryDtoEnvelope**](TenantTerritoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tenant_territory

> models::EmptyEnvelope update_tenant_territory(tenant_id, tenant_territory_id, api_version, x_api_version, tenant_territory_update_dto)
Update a tenant territory

Update a tenant territory

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_territory_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_territory_update_dto** | Option<[**TenantTerritoryUpdateDto**](TenantTerritoryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

