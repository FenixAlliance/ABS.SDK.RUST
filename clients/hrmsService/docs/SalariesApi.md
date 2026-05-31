# \SalariesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_salary_async**](SalariesApi.md#create_salary_async) | **POST** /api/v2/HrmsService/Salaries | Create a salary
[**delete_salary_async**](SalariesApi.md#delete_salary_async) | **DELETE** /api/v2/HrmsService/Salaries/{salaryId} | Delete a salary
[**get_salaries_async**](SalariesApi.md#get_salaries_async) | **GET** /api/v2/HrmsService/Salaries | Get salaries
[**get_salaries_count_async**](SalariesApi.md#get_salaries_count_async) | **GET** /api/v2/HrmsService/Salaries/Count | Count salaries
[**get_salary_by_id_async**](SalariesApi.md#get_salary_by_id_async) | **GET** /api/v2/HrmsService/Salaries/{salaryId} | Get salary by ID
[**update_salary_async**](SalariesApi.md#update_salary_async) | **PUT** /api/v2/HrmsService/Salaries/{salaryId} | Update a salary



## create_salary_async

> models::EmptyEnvelope create_salary_async(tenant_id, api_version, x_api_version, salary_create_dto)
Create a salary

Creates a new salary for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**salary_create_dto** | Option<[**SalaryCreateDto**](SalaryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_salary_async

> models::EmptyEnvelope delete_salary_async(tenant_id, salary_id, api_version, x_api_version)
Delete a salary

Deletes a salary for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**salary_id** | **uuid::Uuid** |  | [required] |
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


## get_salaries_async

> models::SalaryDtoListEnvelope get_salaries_async(tenant_id, api_version, x_api_version)
Get salaries

Retrieves salaries for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SalaryDtoListEnvelope**](SalaryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_salaries_count_async

> models::Int32Envelope get_salaries_count_async(tenant_id, api_version, x_api_version)
Count salaries

Counts salaries for the specified tenant.

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


## get_salary_by_id_async

> models::SalaryDtoEnvelope get_salary_by_id_async(tenant_id, salary_id, api_version, x_api_version)
Get salary by ID

Retrieves a specific salary by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**salary_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SalaryDtoEnvelope**](SalaryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_salary_async

> models::EmptyEnvelope update_salary_async(tenant_id, salary_id, api_version, x_api_version, salary_update_dto)
Update a salary

Updates an existing salary for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**salary_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**salary_update_dto** | Option<[**SalaryUpdateDto**](SalaryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

