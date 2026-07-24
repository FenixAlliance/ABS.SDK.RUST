# \ProjectTasksApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_project_task_async**](ProjectTasksApi.md#create_project_task_async) | **POST** /api/v2/ProjectsService/ProjectTasks | Create a project task
[**delete_project_task_async**](ProjectTasksApi.md#delete_project_task_async) | **DELETE** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Delete a project task
[**get_project_task_by_id_async**](ProjectTasksApi.md#get_project_task_by_id_async) | **GET** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Get project task by ID
[**get_project_tasks_async**](ProjectTasksApi.md#get_project_tasks_async) | **GET** /api/v2/ProjectsService/ProjectTasks | Get all project tasks
[**get_project_tasks_count_async**](ProjectTasksApi.md#get_project_tasks_count_async) | **GET** /api/v2/ProjectsService/ProjectTasks/Count | Get project tasks count
[**patch_project_task_async**](ProjectTasksApi.md#patch_project_task_async) | **PATCH** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Patch a project task
[**update_project_task_async**](ProjectTasksApi.md#update_project_task_async) | **PUT** /api/v2/ProjectsService/ProjectTasks/{projectTaskId} | Update a project task



## create_project_task_async

> models::EmptyEnvelope create_project_task_async(tenant_id, api_version, x_api_version, project_task_create_dto)
Create a project task

Creates a new project task.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_task_create_dto** | Option<[**ProjectTaskCreateDto**](ProjectTaskCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project_task_async

> models::EmptyEnvelope delete_project_task_async(tenant_id, project_task_id, api_version, x_api_version)
Delete a project task

Deletes a project task.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |
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


## get_project_task_by_id_async

> models::ProjectTaskDtoEnvelope get_project_task_by_id_async(tenant_id, project_task_id, api_version, x_api_version)
Get project task by ID

Retrieves a specific project task.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTaskDtoEnvelope**](ProjectTaskDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_tasks_async

> models::ProjectTaskDtoListEnvelope get_project_tasks_async(tenant_id, api_version, x_api_version)
Get all project tasks

Retrieves all project tasks for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTaskDtoListEnvelope**](ProjectTaskDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_tasks_count_async

> models::Int32Envelope get_project_tasks_count_async(tenant_id, api_version, x_api_version)
Get project tasks count

Returns the count of project tasks for the specified tenant.

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


## patch_project_task_async

> models::EmptyEnvelope patch_project_task_async(tenant_id, project_task_id, api_version, x_api_version, operation)
Patch a project task

Partially updates an existing project task.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_task_async

> models::EmptyEnvelope update_project_task_async(tenant_id, project_task_id, api_version, x_api_version, project_task_update_dto)
Update a project task

Updates an existing project task.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_task_update_dto** | Option<[**ProjectTaskUpdateDto**](ProjectTaskUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

