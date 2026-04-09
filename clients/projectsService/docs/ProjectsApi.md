# \ProjectsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_project_async**](ProjectsApi.md#create_project_async) | **POST** /api/v2/ProjectsService/Projects | Creates a new project
[**create_project_period_async**](ProjectsApi.md#create_project_period_async) | **POST** /api/v2/ProjectsService/Projects/{projectId}/Periods | Creates a project period
[**create_project_task_async**](ProjectsApi.md#create_project_task_async) | **POST** /api/v2/ProjectsService/Projects/{projectId}/Tasks | Creates a project task
[**delete_project_async**](ProjectsApi.md#delete_project_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId} | Deletes a project
[**delete_project_period_async**](ProjectsApi.md#delete_project_period_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId}/Periods/{projectPeriodId} | Deletes a project period
[**delete_project_task_async**](ProjectsApi.md#delete_project_task_async) | **DELETE** /api/v2/ProjectsService/Projects/{projectId}/Tasks/{projectTaskId} | Deletes a project task
[**get_project_by_id_async**](ProjectsApi.md#get_project_by_id_async) | **GET** /api/v2/ProjectsService/Projects/{projectId} | Gets a project by ID
[**get_project_periods_async**](ProjectsApi.md#get_project_periods_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Periods | Retrieves project periods
[**get_project_task_categories_async**](ProjectsApi.md#get_project_task_categories_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TaskCategories | Retrieves project task categories
[**get_project_task_categories_count_async**](ProjectsApi.md#get_project_task_categories_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TaskCategories/Count | Counts project task categories
[**get_project_tasks_async**](ProjectsApi.md#get_project_tasks_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Tasks | Retrieves project tasks
[**get_project_tasks_count_async**](ProjectsApi.md#get_project_tasks_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/Tasks/Count | Counts project tasks
[**get_project_time_logs_async**](ProjectsApi.md#get_project_time_logs_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TimeLogs | Retrieves project time logs
[**get_project_time_logs_count_async**](ProjectsApi.md#get_project_time_logs_count_async) | **GET** /api/v2/ProjectsService/Projects/{projectId}/TimeLogs/Count | Counts project time logs
[**get_projects_by_tenant_id_async**](ProjectsApi.md#get_projects_by_tenant_id_async) | **GET** /api/v2/ProjectsService/Projects | Retrieves all projects
[**get_projects_count_by_tenant_id_async**](ProjectsApi.md#get_projects_count_by_tenant_id_async) | **GET** /api/v2/ProjectsService/Projects/Count | Counts projects
[**update_project_async**](ProjectsApi.md#update_project_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId} | Updates a project
[**update_project_period_async**](ProjectsApi.md#update_project_period_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId}/Periods/{projectPeriodId} | Updates a project period
[**update_project_task_async**](ProjectsApi.md#update_project_task_async) | **PUT** /api/v2/ProjectsService/Projects/{projectId}/Tasks/{projectTaskId} | Updates a project task



## create_project_async

> models::EmptyEnvelope create_project_async(tenant_id, project_create_dto)
Creates a new project

Creates a new project for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_create_dto** | Option<[**ProjectCreateDto**](ProjectCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_project_period_async

> models::EmptyEnvelope create_project_period_async(project_id, tenant_id, project_period_create_dto)
Creates a project period

Creates a new period for the specified project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_period_create_dto** | Option<[**ProjectPeriodCreateDto**](ProjectPeriodCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_project_task_async

> models::EmptyEnvelope create_project_task_async(project_id, tenant_id, project_task_create_dto)
Creates a project task

Creates a new task for the specified project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_create_dto** | Option<[**ProjectTaskCreateDto**](ProjectTaskCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project_async

> models::EmptyEnvelope delete_project_async(project_id, tenant_id)
Deletes a project

Deletes the specified project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project_period_async

> models::EmptyEnvelope delete_project_period_async(project_id, project_period_id, tenant_id)
Deletes a project period

Deletes the specified period from a project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**project_period_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project_task_async

> models::EmptyEnvelope delete_project_task_async(tenant_id, project_id, project_task_id)
Deletes a project task

Deletes the specified task from a project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_by_id_async

> models::ProjectDtoEnvelope get_project_by_id_async(project_id, tenant_id)
Gets a project by ID

Retrieves the details of a project using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProjectDtoEnvelope**](ProjectDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_periods_async

> models::ProjectPeriodDtoListEnvelope get_project_periods_async(project_id, tenant_id)
Retrieves project periods

Gets all periods for a specific project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProjectPeriodDtoListEnvelope**](ProjectPeriodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_task_categories_async

> models::TaskCategoryDtoListEnvelope get_project_task_categories_async(project_id, tenant_id)
Retrieves project task categories

Gets all task categories for a specific project with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskCategoryDtoListEnvelope**](TaskCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_task_categories_count_async

> models::Int32Envelope get_project_task_categories_count_async(project_id, tenant_id)
Counts project task categories

Gets the count of task categories for a specific project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_tasks_async

> models::ProjectTaskDtoListEnvelope get_project_tasks_async(project_id, tenant_id)
Retrieves project tasks

Gets all tasks for a specific project with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProjectTaskDtoListEnvelope**](ProjectTaskDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_tasks_count_async

> models::Int32Envelope get_project_tasks_count_async(project_id, tenant_id)
Counts project tasks

Gets the count of tasks for a specific project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_logs_async

> models::ProjectTimeLogDtoListEnvelope get_project_time_logs_async(project_id, tenant_id)
Retrieves project time logs

Gets all time log entries for a specific project with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_logs_count_async

> models::Int32Envelope get_project_time_logs_count_async(project_id, tenant_id)
Counts project time logs

Gets the count of time log entries for a specific project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_projects_by_tenant_id_async

> models::ProjectDtoListEnvelope get_projects_by_tenant_id_async(tenant_id)
Retrieves all projects

Gets all projects for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProjectDtoListEnvelope**](ProjectDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_projects_count_by_tenant_id_async

> models::Int32Envelope get_projects_count_by_tenant_id_async(tenant_id)
Counts projects

Gets the count of projects for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_async

> models::EmptyEnvelope update_project_async(project_id, tenant_id, project_update_dto)
Updates a project

Updates the specified project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_update_dto** | Option<[**ProjectUpdateDto**](ProjectUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_period_async

> models::EmptyEnvelope update_project_period_async(project_id, project_period_id, tenant_id, project_period_update_dto)
Updates a project period

Updates the specified period for a project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**project_period_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_period_update_dto** | Option<[**ProjectPeriodUpdateDto**](ProjectPeriodUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_task_async

> models::EmptyEnvelope update_project_task_async(project_id, project_task_id, tenant_id, project_task_update_dto)
Updates a project task

Updates the specified task in a project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**project_task_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_task_update_dto** | Option<[**ProjectTaskUpdateDto**](ProjectTaskUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

