# \TaxRatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tax_rate**](TaxRatesApi.md#create_tax_rate) | **POST** /api/v2/AccountingService/TaxRates | Create a tax rate
[**delete_tax_rate**](TaxRatesApi.md#delete_tax_rate) | **DELETE** /api/v2/AccountingService/TaxRates/{id} | Delete a tax rate
[**get_tax_rate**](TaxRatesApi.md#get_tax_rate) | **GET** /api/v2/AccountingService/TaxRates/{id} | Get tax rate by ID
[**get_tax_rates**](TaxRatesApi.md#get_tax_rates) | **GET** /api/v2/AccountingService/TaxRates | Get all tax rates for a tenant
[**get_tax_rates_count**](TaxRatesApi.md#get_tax_rates_count) | **GET** /api/v2/AccountingService/TaxRates/Count | Get tax rates count
[**update_tax_rate**](TaxRatesApi.md#update_tax_rate) | **PUT** /api/v2/AccountingService/TaxRates/{id} | Update a tax rate



## create_tax_rate

> models::EmptyEnvelope create_tax_rate(tenant_id, api_version, x_api_version, tax_rate_create_dto)
Create a tax rate

Creates a new tax rate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_rate_create_dto** | Option<[**TaxRateCreateDto**](TaxRateCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tax_rate

> models::EmptyEnvelope delete_tax_rate(tenant_id, id, api_version, x_api_version)
Delete a tax rate

Deletes a tax rate identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_tax_rate

> models::TaxRateDtoEnvelope get_tax_rate(tenant_id, id, api_version, x_api_version)
Get tax rate by ID

Retrieves a specific tax rate by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxRateDtoEnvelope**](TaxRateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_rates

> models::TaxRateDtoListEnvelope get_tax_rates(tenant_id, api_version, x_api_version)
Get all tax rates for a tenant

Retrieves all tax rates for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxRateDtoListEnvelope**](TaxRateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_rates_count

> models::Int32Envelope get_tax_rates_count(tenant_id, api_version, x_api_version)
Get tax rates count

Returns the count of tax rates for the specified tenant.

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


## update_tax_rate

> models::EmptyEnvelope update_tax_rate(tenant_id, id, api_version, x_api_version, tax_rate_update_dto)
Update a tax rate

Updates an existing tax rate identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_rate_update_dto** | Option<[**TaxRateUpdateDto**](TaxRateUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

