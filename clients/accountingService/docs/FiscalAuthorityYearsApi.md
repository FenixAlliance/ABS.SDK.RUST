# \FiscalAuthorityYearsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_year**](FiscalAuthorityYearsApi.md#create_fiscal_year) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears | Create a fiscal year
[**delete_fiscal_year**](FiscalAuthorityYearsApi.md#delete_fiscal_year) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears/{fiscalYearId} | Delete a fiscal year
[**get_fiscal_year**](FiscalAuthorityYearsApi.md#get_fiscal_year) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId} | Get fiscal year by ID for an authority
[**get_fiscal_years**](FiscalAuthorityYearsApi.md#get_fiscal_years) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalYears | Get fiscal years for an authority
[**get_fiscal_years_count**](FiscalAuthorityYearsApi.md#get_fiscal_years_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/Count | Get fiscal years count for an authority
[**update_fiscal_year**](FiscalAuthorityYearsApi.md#update_fiscal_year) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalYears/{fiscalYearId} | Update a fiscal year



## create_fiscal_year

> models::EmptyEnvelope create_fiscal_year(tenant_id, api_version, x_api_version, fiscal_year_create_dto)
Create a fiscal year

Creates a new fiscal year associated with a fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_year_create_dto** | Option<[**FiscalYearCreateDto**](FiscalYearCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_year

> models::EmptyEnvelope delete_fiscal_year(tenant_id, fiscal_year_id, api_version, x_api_version)
Delete a fiscal year

Deletes a fiscal year identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_year

> models::FiscalYearDtoEnvelope get_fiscal_year(tenant_id, fiscal_authority_id, fiscal_year_id, api_version, x_api_version)
Get fiscal year by ID for an authority

Retrieves a specific fiscal year by its unique identifier within a fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalYearDtoEnvelope**](FiscalYearDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_years

> models::FiscalYearDtoListEnvelope get_fiscal_years(tenant_id, fiscal_authority_id, authority_id, api_version, x_api_version)
Get fiscal years for an authority

Retrieves all fiscal years associated with the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalYearDtoListEnvelope**](FiscalYearDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_years_count

> models::Int32Envelope get_fiscal_years_count(tenant_id, fiscal_authority_id, api_version, x_api_version)
Get fiscal years count for an authority

Returns the total count of fiscal years for the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
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


## update_fiscal_year

> models::EmptyEnvelope update_fiscal_year(tenant_id, fiscal_year_id, api_version, x_api_version, fiscal_year_update_dto)
Update a fiscal year

Updates an existing fiscal year identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_year_update_dto** | Option<[**FiscalYearUpdateDto**](FiscalYearUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

