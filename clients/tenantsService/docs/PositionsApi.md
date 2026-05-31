# \PositionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_position**](PositionsApi.md#create_tenant_position) | **POST** /api/v2/TenantsService/Positions | Create a new tenant position
[**delete_tenant_position**](PositionsApi.md#delete_tenant_position) | **DELETE** /api/v2/TenantsService/Positions/{tenantPositionId} | Delete a tenant position
[**get_tenant_position_by_id**](PositionsApi.md#get_tenant_position_by_id) | **GET** /api/v2/TenantsService/Positions/{tenantPositionId} | Retrieve a single tenant position by its ID
[**get_tenant_positions**](PositionsApi.md#get_tenant_positions) | **GET** /api/v2/TenantsService/Positions | Retrieve a list of tenant positions
[**get_tenant_positions_count**](PositionsApi.md#get_tenant_positions_count) | **GET** /api/v2/TenantsService/Positions/Count | Get the count of tenant positions
[**update_tenant_position**](PositionsApi.md#update_tenant_position) | **PUT** /api/v2/TenantsService/Positions/{tenantPositionId} | Update a tenant position



## create_tenant_position

> models::EmptyEnvelope create_tenant_position(tenant_id, api_version, x_api_version, tenant_position_create_dto)
Create a new tenant position

Create a new tenant position

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_position_create_dto** | Option<[**TenantPositionCreateDto**](TenantPositionCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_position

> models::EmptyEnvelope delete_tenant_position(tenant_id, tenant_position_id, api_version, x_api_version)
Delete a tenant position

Delete a tenant position

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_position_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_position_by_id

> models::TenantPositionDtoEnvelope get_tenant_position_by_id(tenant_id, tenant_position_id, api_version, x_api_version)
Retrieve a single tenant position by its ID

Retrieve a single tenant position by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_position_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantPositionDtoEnvelope**](TenantPositionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_positions

> models::TenantPositionDtoListEnvelope get_tenant_positions(tenant_id, api_version, x_api_version)
Retrieve a list of tenant positions

Retrieve a list of tenant positions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantPositionDtoListEnvelope**](TenantPositionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_positions_count

> models::Int32Envelope get_tenant_positions_count(tenant_id, api_version, x_api_version)
Get the count of tenant positions

Get the count of tenant positions

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


## update_tenant_position

> models::EmptyEnvelope update_tenant_position(tenant_id, tenant_position_id, api_version, x_api_version, tenant_position_update_dto)
Update a tenant position

Update a tenant position

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_position_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_position_update_dto** | Option<[**TenantPositionUpdateDto**](TenantPositionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

