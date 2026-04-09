# \FiscalAuthoritiesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_authority**](FiscalAuthoritiesApi.md#create_fiscal_authority) | **POST** /api/v2/AccountingService/Fiscals/Authorities | Create a fiscal authority
[**delete_fiscal_authority**](FiscalAuthoritiesApi.md#delete_fiscal_authority) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Delete a fiscal authority
[**get_fiscal_authorities**](FiscalAuthoritiesApi.md#get_fiscal_authorities) | **GET** /api/v2/AccountingService/Fiscals/Authorities | Get fiscal authorities
[**get_fiscal_authorities_count**](FiscalAuthoritiesApi.md#get_fiscal_authorities_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/Count | Get fiscal authorities count
[**get_fiscal_authority**](FiscalAuthoritiesApi.md#get_fiscal_authority) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Get fiscal authority by ID
[**update_fiscal_authority**](FiscalAuthoritiesApi.md#update_fiscal_authority) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/{authorityId} | Update a fiscal authority



## create_fiscal_authority

> models::EmptyEnvelope create_fiscal_authority(tenant_id, api_version, x_api_version, fiscal_authority_create_dto)
Create a fiscal authority

Creates a new fiscal authority for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_authority_create_dto** | Option<[**FiscalAuthorityCreateDto**](FiscalAuthorityCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_authority

> models::EmptyEnvelope delete_fiscal_authority(tenant_id, authority_id, api_version, x_api_version)
Delete a fiscal authority

Deletes a fiscal authority identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_authorities

> models::FiscalAuthorityDtoListEnvelope get_fiscal_authorities(tenant_id, api_version, x_api_version)
Get fiscal authorities

Retrieves all fiscal authorities for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalAuthorityDtoListEnvelope**](FiscalAuthorityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_authorities_count

> models::Int32Envelope get_fiscal_authorities_count(tenant_id, api_version, x_api_version)
Get fiscal authorities count

Returns the total count of fiscal authorities for the specified tenant.

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


## get_fiscal_authority

> models::FiscalAuthorityDtoEnvelope get_fiscal_authority(tenant_id, authority_id, api_version, x_api_version)
Get fiscal authority by ID

Retrieves a specific fiscal authority by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalAuthorityDtoEnvelope**](FiscalAuthorityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_fiscal_authority

> models::EmptyEnvelope update_fiscal_authority(tenant_id, authority_id, api_version, x_api_version, fiscal_authority_update_dto)
Update a fiscal authority

Updates an existing fiscal authority identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_authority_update_dto** | Option<[**FiscalAuthorityUpdateDto**](FiscalAuthorityUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

