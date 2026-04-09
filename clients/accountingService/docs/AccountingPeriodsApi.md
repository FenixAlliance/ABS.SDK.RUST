# \AccountingPeriodsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_accounting_period**](AccountingPeriodsApi.md#create_accounting_period) | **POST** /api/v2/AccountingService/AccountingPeriods | Creates a new accounting period
[**delete_accounting_period**](AccountingPeriodsApi.md#delete_accounting_period) | **DELETE** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Deletes an existing accounting period
[**get_accounting_period**](AccountingPeriodsApi.md#get_accounting_period) | **GET** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Gets the current tenant accounting period
[**get_accounting_periods**](AccountingPeriodsApi.md#get_accounting_periods) | **GET** /api/v2/AccountingService/AccountingPeriods | Get all accounting periods for a tenant
[**get_accounting_periods_count_async**](AccountingPeriodsApi.md#get_accounting_periods_count_async) | **GET** /api/v2/AccountingService/AccountingPeriods/Count | Gets the current tenant accounting periods count
[**update_accounting_period**](AccountingPeriodsApi.md#update_accounting_period) | **PUT** /api/v2/AccountingService/AccountingPeriods/{accountingPeriodId} | Updates an existing accounting period



## create_accounting_period

> models::EmptyEnvelope create_accounting_period(tenant_id, api_version, x_api_version, accounting_period_create_dto)
Creates a new accounting period

Creates a new accounting period.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_period_create_dto** | Option<[**AccountingPeriodCreateDto**](AccountingPeriodCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_accounting_period

> models::EmptyEnvelope delete_accounting_period(tenant_id, accounting_period_id, api_version, x_api_version)
Deletes an existing accounting period

Deletes an existing accounting period.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**accounting_period_id** | **uuid::Uuid** |  | [required] |
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


## get_accounting_period

> models::AccountingPeriodDtoEnvelope get_accounting_period(tenant_id, accounting_period_id, api_version, x_api_version)
Gets the current tenant accounting period

Get the currently acting tenant accounting period.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**accounting_period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingPeriodDtoEnvelope**](AccountingPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_accounting_periods

> models::AccountingPeriodDtoListEnvelope get_accounting_periods(tenant_id, api_version, x_api_version)
Get all accounting periods for a tenant

Retrieves all accounting periods for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingPeriodDtoListEnvelope**](AccountingPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_accounting_periods_count_async

> models::Int32Envelope get_accounting_periods_count_async(tenant_id, api_version, x_api_version)
Gets the current tenant accounting periods count

Get the currently acting tenant accounting periods count.

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


## update_accounting_period

> models::EmptyEnvelope update_accounting_period(tenant_id, accounting_period_id, api_version, x_api_version, accounting_period_update_dto)
Updates an existing accounting period

Updates an existing accounting period.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**accounting_period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_period_update_dto** | Option<[**AccountingPeriodUpdateDto**](AccountingPeriodUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

