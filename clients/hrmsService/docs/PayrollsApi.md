# \PayrollsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payroll_async**](PayrollsApi.md#create_payroll_async) | **POST** /api/v2/HrmsService/Payrolls | Create a payroll
[**delete_payroll_async**](PayrollsApi.md#delete_payroll_async) | **DELETE** /api/v2/HrmsService/Payrolls/{payrollId} | Delete a payroll
[**get_payroll_by_id_async**](PayrollsApi.md#get_payroll_by_id_async) | **GET** /api/v2/HrmsService/Payrolls/{payrollId} | Get payroll by ID
[**get_payrolls_async**](PayrollsApi.md#get_payrolls_async) | **GET** /api/v2/HrmsService/Payrolls | Get payrolls
[**get_payrolls_count_async**](PayrollsApi.md#get_payrolls_count_async) | **GET** /api/v2/HrmsService/Payrolls/Count | Count payrolls
[**update_payroll_async**](PayrollsApi.md#update_payroll_async) | **PUT** /api/v2/HrmsService/Payrolls/{payrollId} | Update a payroll



## create_payroll_async

> models::EmptyEnvelope create_payroll_async(tenant_id, api_version, x_api_version, payroll_create_dto)
Create a payroll

Creates a new payroll for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payroll_create_dto** | Option<[**PayrollCreateDto**](PayrollCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payroll_async

> models::EmptyEnvelope delete_payroll_async(tenant_id, payroll_id, api_version, x_api_version)
Delete a payroll

Deletes a payroll for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payroll_id** | **uuid::Uuid** |  | [required] |
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


## get_payroll_by_id_async

> models::PayrollDtoEnvelope get_payroll_by_id_async(tenant_id, payroll_id, api_version, x_api_version)
Get payroll by ID

Retrieves a specific payroll by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payroll_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PayrollDtoEnvelope**](PayrollDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payrolls_async

> models::PayrollDtoListEnvelope get_payrolls_async(tenant_id, api_version, x_api_version)
Get payrolls

Retrieves payrolls for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PayrollDtoListEnvelope**](PayrollDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payrolls_count_async

> models::Int32Envelope get_payrolls_count_async(tenant_id, api_version, x_api_version)
Count payrolls

Counts payrolls for the specified tenant.

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


## update_payroll_async

> models::EmptyEnvelope update_payroll_async(tenant_id, payroll_id, api_version, x_api_version, payroll_update_dto)
Update a payroll

Updates an existing payroll for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payroll_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payroll_update_dto** | Option<[**PayrollUpdateDto**](PayrollUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

