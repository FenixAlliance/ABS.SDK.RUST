# \TaskTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_task_type_async**](TaskTypesApi.md#create_task_type_async) | **POST** /api/v2/ProjectsService/TaskTypes | Creates a new task type
[**delete_task_type_async**](TaskTypesApi.md#delete_task_type_async) | **DELETE** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Deletes a task type
[**get_task_type_by_id_async**](TaskTypesApi.md#get_task_type_by_id_async) | **GET** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Gets a task type by ID
[**update_task_type_async**](TaskTypesApi.md#update_task_type_async) | **PUT** /api/v2/ProjectsService/TaskTypes/{taskTypeId} | Updates a task type



## create_task_type_async

> models::TaskTypeDto create_task_type_async(tenant_id, task_type_create_dto)
Creates a new task type

Creates a new task type for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**task_type_create_dto** | Option<[**TaskTypeCreateDto**](TaskTypeCreateDto.md)> |  |  |

### Return type

[**models::TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_task_type_async

> models::TaskTypeDto delete_task_type_async(task_type_id, tenant_id)
Deletes a task type

Deletes the specified task type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_type_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_task_type_by_id_async

> models::TaskTypeDto get_task_type_by_id_async(task_type_id, tenant_id)
Gets a task type by ID

Retrieves the details of a task type using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_type_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_task_type_async

> models::TaskTypeDto update_task_type_async(task_type_id, tenant_id, task_type_update_dto)
Updates a task type

Updates the specified task type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_type_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**task_type_update_dto** | Option<[**TaskTypeUpdateDto**](TaskTypeUpdateDto.md)> |  |  |

### Return type

[**models::TaskTypeDto**](TaskTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

