# \FiscalRegimesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_regime**](FiscalRegimesApi.md#create_fiscal_regime) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes | Create a fiscal regime
[**delete_fiscal_regime**](FiscalRegimesApi.md#delete_fiscal_regime) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes/{regimeId} | Delete a fiscal regime
[**get_fiscal_regime**](FiscalRegimesApi.md#get_fiscal_regime) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalRegimes/{regimeId} | Get fiscal regime by ID
[**get_fiscal_regimes**](FiscalRegimesApi.md#get_fiscal_regimes) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalRegimes | Get fiscal regimes for an authority
[**get_fiscal_regimes_count**](FiscalRegimesApi.md#get_fiscal_regimes_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalRegimes/Count | Get fiscal regimes count
[**update_fiscal_regime**](FiscalRegimesApi.md#update_fiscal_regime) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalRegimes/{regimeId} | Update a fiscal regime



## create_fiscal_regime

> models::EmptyEnvelope create_fiscal_regime(tenant_id, api_version, x_api_version, fiscal_regime_create_dto)
Create a fiscal regime

Creates a new fiscal regime for a fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_regime_create_dto** | Option<[**FiscalRegimeCreateDto**](FiscalRegimeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_regime

> models::EmptyEnvelope delete_fiscal_regime(tenant_id, regime_id, api_version, x_api_version)
Delete a fiscal regime

Deletes a fiscal regime identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**regime_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_regime

> models::FiscalRegimeDtoEnvelope get_fiscal_regime(tenant_id, fiscal_authority_id, regime_id, api_version, x_api_version)
Get fiscal regime by ID

Retrieves a specific fiscal regime by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**regime_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalRegimeDtoEnvelope**](FiscalRegimeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_regimes

> models::FiscalRegimeDtoListEnvelope get_fiscal_regimes(fiscal_authority_id, authority_id, api_version, x_api_version)
Get fiscal regimes for an authority

Retrieves all fiscal regimes for the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalRegimeDtoListEnvelope**](FiscalRegimeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_regimes_count

> models::Int32Envelope get_fiscal_regimes_count(fiscal_authority_id, api_version, x_api_version)
Get fiscal regimes count

Returns the total count of fiscal regimes for the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
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


## update_fiscal_regime

> models::EmptyEnvelope update_fiscal_regime(tenant_id, regime_id, api_version, x_api_version, fiscal_regime_update_dto)
Update a fiscal regime

Updates an existing fiscal regime identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**regime_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_regime_update_dto** | Option<[**FiscalRegimeUpdateDto**](FiscalRegimeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

