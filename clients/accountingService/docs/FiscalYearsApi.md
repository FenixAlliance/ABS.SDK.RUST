# \FiscalYearsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_year_async**](FiscalYearsApi.md#create_fiscal_year_async) | **POST** /api/v2/AccountingService/FiscalYears | Create fiscal year
[**delete_fiscal_year_async**](FiscalYearsApi.md#delete_fiscal_year_async) | **DELETE** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Delete fiscal year
[**get_fiscal_year_details_async**](FiscalYearsApi.md#get_fiscal_year_details_async) | **GET** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Get fiscal year by ID
[**get_fiscal_years_async**](FiscalYearsApi.md#get_fiscal_years_async) | **GET** /api/v2/AccountingService/FiscalYears | Get all fiscal years
[**get_fiscal_years_count_async**](FiscalYearsApi.md#get_fiscal_years_count_async) | **GET** /api/v2/AccountingService/FiscalYears/Count | Count fiscal years
[**update_fiscal_year_async**](FiscalYearsApi.md#update_fiscal_year_async) | **PUT** /api/v2/AccountingService/FiscalYears/{fiscalYearId} | Update fiscal year



## create_fiscal_year_async

> models::EmptyEnvelope create_fiscal_year_async(tenant_id, api_version, x_api_version, fiscal_year_create_dto)
Create fiscal year

Creates a new fiscal year entry for a tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## delete_fiscal_year_async

> models::EmptyEnvelope delete_fiscal_year_async(tenant_id, fiscal_year_id, api_version, x_api_version)
Delete fiscal year

Deletes a fiscal year identified by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_year_details_async

> models::FiscalYearDtoEnvelope get_fiscal_year_details_async(tenant_id, fiscal_year_id, api_version, x_api_version)
Get fiscal year by ID

Gets details for a specific fiscal year.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_years_async

> models::FiscalYearDtoIReadOnlyListEnvelope get_fiscal_years_async(tenant_id, api_version, x_api_version)
Get all fiscal years

Retrieves a list of fiscal years for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalYearDtoIReadOnlyListEnvelope**](FiscalYearDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_years_count_async

> models::Int32Envelope get_fiscal_years_count_async(tenant_id, api_version, x_api_version)
Count fiscal years

Returns the number of fiscal years for a tenant.

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


## update_fiscal_year_async

> models::EmptyEnvelope update_fiscal_year_async(tenant_id, fiscal_year_id, api_version, x_api_version, fiscal_year_update_dto)
Update fiscal year

Updates an existing fiscal year identified by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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

