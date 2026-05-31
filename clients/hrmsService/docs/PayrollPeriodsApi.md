# \PayrollPeriodsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payroll_period_async**](PayrollPeriodsApi.md#create_payroll_period_async) | **POST** /api/v2/HrmsService/PayrollPeriods | Create a payroll period
[**delete_payroll_period_async**](PayrollPeriodsApi.md#delete_payroll_period_async) | **DELETE** /api/v2/HrmsService/PayrollPeriods/{periodId} | Delete a payroll period
[**get_payroll_period_by_id_async**](PayrollPeriodsApi.md#get_payroll_period_by_id_async) | **GET** /api/v2/HrmsService/PayrollPeriods/{periodId} | Get payroll period by ID
[**get_payroll_periods_async**](PayrollPeriodsApi.md#get_payroll_periods_async) | **GET** /api/v2/HrmsService/PayrollPeriods | Get payroll periods
[**get_payroll_periods_count_async**](PayrollPeriodsApi.md#get_payroll_periods_count_async) | **GET** /api/v2/HrmsService/PayrollPeriods/Count | Count payroll periods
[**update_payroll_period_async**](PayrollPeriodsApi.md#update_payroll_period_async) | **PUT** /api/v2/HrmsService/PayrollPeriods/{periodId} | Update a payroll period



## create_payroll_period_async

> models::EmptyEnvelope create_payroll_period_async(tenant_id, api_version, x_api_version, payroll_period_create_dto)
Create a payroll period

Creates a new payroll period for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payroll_period_create_dto** | Option<[**PayrollPeriodCreateDto**](PayrollPeriodCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payroll_period_async

> models::EmptyEnvelope delete_payroll_period_async(tenant_id, period_id, api_version, x_api_version)
Delete a payroll period

Deletes a payroll period for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**period_id** | **uuid::Uuid** |  | [required] |
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


## get_payroll_period_by_id_async

> models::PayrollPeriodDtoEnvelope get_payroll_period_by_id_async(tenant_id, period_id, api_version, x_api_version)
Get payroll period by ID

Retrieves a specific payroll period by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PayrollPeriodDtoEnvelope**](PayrollPeriodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payroll_periods_async

> models::PayrollPeriodDtoListEnvelope get_payroll_periods_async(tenant_id, api_version, x_api_version)
Get payroll periods

Retrieves payroll periods for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PayrollPeriodDtoListEnvelope**](PayrollPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payroll_periods_count_async

> models::Int32Envelope get_payroll_periods_count_async(tenant_id, api_version, x_api_version)
Count payroll periods

Counts payroll periods for the specified tenant.

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


## update_payroll_period_async

> models::EmptyEnvelope update_payroll_period_async(tenant_id, period_id, api_version, x_api_version, payroll_period_update_dto)
Update a payroll period

Updates an existing payroll period for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payroll_period_update_dto** | Option<[**PayrollPeriodUpdateDto**](PayrollPeriodUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

