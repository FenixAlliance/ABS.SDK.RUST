# \EmployeeTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_employee_type_async**](EmployeeTypesApi.md#create_employee_type_async) | **POST** /api/v2/HrmsService/EmployeeTypes | Create an employee type
[**delete_employee_type_async**](EmployeeTypesApi.md#delete_employee_type_async) | **DELETE** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Delete an employee type
[**get_employee_type_by_id_async**](EmployeeTypesApi.md#get_employee_type_by_id_async) | **GET** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Get employee type by ID
[**get_employee_types_async**](EmployeeTypesApi.md#get_employee_types_async) | **GET** /api/v2/HrmsService/EmployeeTypes | Get employee types
[**get_employee_types_count_async**](EmployeeTypesApi.md#get_employee_types_count_async) | **GET** /api/v2/HrmsService/EmployeeTypes/Count | Count employee types
[**update_employee_type_async**](EmployeeTypesApi.md#update_employee_type_async) | **PUT** /api/v2/HrmsService/EmployeeTypes/{employeeTypeId} | Update an employee type



## create_employee_type_async

> models::EmptyEnvelope create_employee_type_async(tenant_id, api_version, x_api_version, employee_type_create_dto)
Create an employee type

Creates a new employee type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**employee_type_create_dto** | Option<[**EmployeeTypeCreateDto**](EmployeeTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_employee_type_async

> models::EmptyEnvelope delete_employee_type_async(tenant_id, employee_type_id, api_version, x_api_version)
Delete an employee type

Deletes an employee type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_type_id** | **uuid::Uuid** |  | [required] |
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


## get_employee_type_by_id_async

> models::EmployeeTypeDtoEnvelope get_employee_type_by_id_async(tenant_id, employee_type_id, api_version, x_api_version)
Get employee type by ID

Retrieves a specific employee type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeTypeDtoEnvelope**](EmployeeTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employee_types_async

> models::EmployeeTypeDtoListEnvelope get_employee_types_async(tenant_id, api_version, x_api_version)
Get employee types

Retrieves employee types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeTypeDtoListEnvelope**](EmployeeTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employee_types_count_async

> models::Int32Envelope get_employee_types_count_async(tenant_id, api_version, x_api_version)
Count employee types

Counts employee types for the specified tenant.

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


## update_employee_type_async

> models::EmptyEnvelope update_employee_type_async(tenant_id, employee_type_id, api_version, x_api_version, employee_type_update_dto)
Update an employee type

Updates an existing employee type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**employee_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**employee_type_update_dto** | Option<[**EmployeeTypeUpdateDto**](EmployeeTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

