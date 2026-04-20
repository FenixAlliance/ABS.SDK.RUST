# \DepartmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_department**](DepartmentsApi.md#create_tenant_department) | **POST** /api/v2/TenantsService/Departments | Create a new tenant department
[**delete_tenant_department**](DepartmentsApi.md#delete_tenant_department) | **DELETE** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Delete a tenant department
[**get_tenant_department_by_id**](DepartmentsApi.md#get_tenant_department_by_id) | **GET** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Retrieve a single tenant department by its ID
[**get_tenant_departments**](DepartmentsApi.md#get_tenant_departments) | **GET** /api/v2/TenantsService/Departments | Retrieve a list of tenant departments
[**get_tenant_departments_count**](DepartmentsApi.md#get_tenant_departments_count) | **GET** /api/v2/TenantsService/Departments/Count | Get the count of tenant departments
[**update_tenant_department**](DepartmentsApi.md#update_tenant_department) | **PUT** /api/v2/TenantsService/Departments/{tenantDepartmentId} | Update a tenant department



## create_tenant_department

> models::EmptyEnvelope create_tenant_department(tenant_id, api_version, x_api_version, tenant_department_create_dto)
Create a new tenant department

Create a new tenant department

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_department_create_dto** | Option<[**TenantDepartmentCreateDto**](TenantDepartmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_department

> models::EmptyEnvelope delete_tenant_department(tenant_id, tenant_department_id, api_version, x_api_version)
Delete a tenant department

Delete a tenant department

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_department_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_department_by_id

> models::TenantDepartmentDtoEnvelope get_tenant_department_by_id(tenant_id, tenant_department_id, api_version, x_api_version)
Retrieve a single tenant department by its ID

Retrieve a single tenant department by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_department_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDepartmentDtoEnvelope**](TenantDepartmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_departments

> models::TenantDepartmentDtoListEnvelope get_tenant_departments(tenant_id, api_version, x_api_version)
Retrieve a list of tenant departments

Retrieve a list of tenant departments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDepartmentDtoListEnvelope**](TenantDepartmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_departments_count

> models::Int32Envelope get_tenant_departments_count(tenant_id, api_version, x_api_version)
Get the count of tenant departments

Get the count of tenant departments

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


## update_tenant_department

> models::EmptyEnvelope update_tenant_department(tenant_id, tenant_department_id, api_version, x_api_version, tenant_department_update_dto)
Update a tenant department

Update a tenant department

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_department_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_department_update_dto** | Option<[**TenantDepartmentUpdateDto**](TenantDepartmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

