# \EmployeesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_employee_async**](EmployeesApi.md#create_employee_async) | **POST** /api/v2/HrmsService/Employees | Create an employee
[**delete_employee_async**](EmployeesApi.md#delete_employee_async) | **DELETE** /api/v2/HrmsService/Employees/{employeeId} | Delete an employee
[**get_employee_by_id_async**](EmployeesApi.md#get_employee_by_id_async) | **GET** /api/v2/HrmsService/Employees/{employeeId} | Get employee by ID
[**get_employees_async**](EmployeesApi.md#get_employees_async) | **GET** /api/v2/HrmsService/Employees | Get employees
[**get_employees_count_async**](EmployeesApi.md#get_employees_count_async) | **GET** /api/v2/HrmsService/Employees/Count | Count employees
[**update_employee_async**](EmployeesApi.md#update_employee_async) | **PUT** /api/v2/HrmsService/Employees/{employeeId} | Update an employee



## create_employee_async

> models::EmptyEnvelope create_employee_async(tenant_id, api_version, x_api_version, employee_profile_create_dto)
Create an employee

Creates a new employee for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**employee_profile_create_dto** | Option<[**EmployeeProfileCreateDto**](EmployeeProfileCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_employee_async

> models::EmptyEnvelope delete_employee_async(tenant_id, employee_id, api_version, x_api_version)
Delete an employee

Deletes an employee for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_id** | **uuid::Uuid** |  | [required] |
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


## get_employee_by_id_async

> models::EmployeeProfileDtoEnvelope get_employee_by_id_async(tenant_id, employee_id, api_version, x_api_version)
Get employee by ID

Retrieves a specific employee by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeProfileDtoEnvelope**](EmployeeProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employees_async

> models::EmployeeProfileDtoListEnvelope get_employees_async(tenant_id, api_version, x_api_version)
Get employees

Retrieves employees for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeProfileDtoListEnvelope**](EmployeeProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employees_count_async

> models::Int32Envelope get_employees_count_async(tenant_id, api_version, x_api_version)
Count employees

Counts employees for the specified tenant.

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


## update_employee_async

> models::EmptyEnvelope update_employee_async(tenant_id, employee_id, api_version, x_api_version, body)
Update an employee

Updates an existing employee for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**body** | Option<**serde_json::Value**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

