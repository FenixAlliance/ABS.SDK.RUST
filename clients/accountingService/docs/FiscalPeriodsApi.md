# \FiscalPeriodsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_period**](FiscalPeriodsApi.md#create_fiscal_period) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods | Create a fiscal period
[**delete_fiscal_period**](FiscalPeriodsApi.md#delete_fiscal_period) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods/{fiscalPeriodId} | Delete a fiscal period
[**get_fiscal_period**](FiscalPeriodsApi.md#get_fiscal_period) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods/{fiscalPeriodId} | Get fiscal period by ID
[**get_fiscal_periods**](FiscalPeriodsApi.md#get_fiscal_periods) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods | Get fiscal periods for a fiscal year
[**get_fiscal_periods_count**](FiscalPeriodsApi.md#get_fiscal_periods_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalYears/{fiscalYearId}/FiscalPeriods/Count | Get fiscal periods count
[**update_fiscal_period**](FiscalPeriodsApi.md#update_fiscal_period) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalPeriods/{fiscalPeriodId} | Update a fiscal period



## create_fiscal_period

> models::EmptyEnvelope create_fiscal_period(tenant_id, api_version, x_api_version, fiscal_period_create_dto)
Create a fiscal period

Creates a new fiscal period associated with a fiscal year.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_period_create_dto** | Option<[**FiscalPeriodCreateDto**](FiscalPeriodCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_period

> models::EmptyEnvelope delete_fiscal_period(tenant_id, fiscal_period_id, api_version, x_api_version)
Delete a fiscal period

Deletes a fiscal period identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_period_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_period

> models::FiscalPeriodDtoEnvelope get_fiscal_period(tenant_id, fiscal_authority_id, fiscal_year_id, fiscal_period_id, api_version, x_api_version)
Get fiscal period by ID

Retrieves a specific fiscal period by its unique identifier within a fiscal year.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
**fiscal_period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalPeriodDtoEnvelope**](FiscalPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_periods

> models::FiscalPeriodDtoListEnvelope get_fiscal_periods(tenant_id, fiscal_authority_id, fiscal_year_id, authority_id, api_version, x_api_version)
Get fiscal periods for a fiscal year

Retrieves all fiscal periods for the specified fiscal year within a fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalPeriodDtoListEnvelope**](FiscalPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_periods_count

> models::Int32Envelope get_fiscal_periods_count(tenant_id, fiscal_authority_id, fiscal_year_id, api_version, x_api_version)
Get fiscal periods count

Returns the total count of fiscal periods for the specified fiscal year.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_year_id** | **uuid::Uuid** |  | [required] |
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


## update_fiscal_period

> models::EmptyEnvelope update_fiscal_period(tenant_id, fiscal_period_id, api_version, x_api_version, fiscal_period_update_dto)
Update a fiscal period

Updates an existing fiscal period identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_period_update_dto** | Option<[**FiscalPeriodUpdateDto**](FiscalPeriodUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

