# \ProjectTimeLogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_project_period_time_logs_async**](ProjectTimeLogsApi.md#count_project_period_time_logs_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs/Count | Get the count of project period time logs
[**create_project_time_log_async**](ProjectTimeLogsApi.md#create_project_time_log_async) | **POST** /api/v2/TimeTrackerService/ProjectTimeLogs | Create a new project time log
[**delete_project_time_log_async**](ProjectTimeLogsApi.md#delete_project_time_log_async) | **DELETE** /api/v2/TimeTrackerService/ProjectTimeLogs/{timeLogId} | Delete a project time log
[**get_project_period_time_logs_async**](ProjectTimeLogsApi.md#get_project_period_time_logs_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs | Retrieve project period time logs
[**get_project_time_log_by_id_async**](ProjectTimeLogsApi.md#get_project_time_log_by_id_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs/{timeLogId} | Retrieve a project time log by ID
[**get_project_time_logs_async**](ProjectTimeLogsApi.md#get_project_time_logs_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs/ForProject/{projectId} | Retrieve time logs for a project
[**get_project_time_logs_by_responsible_contact_async**](ProjectTimeLogsApi.md#get_project_time_logs_by_responsible_contact_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs/ByResponsibleContact | Retrieve time logs by responsible contact
[**get_project_time_logs_created_by_contact_async**](ProjectTimeLogsApi.md#get_project_time_logs_created_by_contact_async) | **GET** /api/v2/TimeTrackerService/ProjectTimeLogs/CreatedByContact | Retrieve time logs created by a contact
[**update_project_time_log_async**](ProjectTimeLogsApi.md#update_project_time_log_async) | **PUT** /api/v2/TimeTrackerService/ProjectTimeLogs/{timeLogId} | Update a project time log



## count_project_period_time_logs_async

> models::Int32Envelope count_project_period_time_logs_async(tenant_id, project_period_id, api_version, x_api_version)
Get the count of project period time logs

Returns the total count of time logs for a specific project period with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_period_id** | **uuid::Uuid** |  | [required] |
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


## create_project_time_log_async

> create_project_time_log_async(tenant_id, api_version, x_api_version, project_time_log_create_dto)
Create a new project time log

Creates a new project time log entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_time_log_create_dto** | Option<[**ProjectTimeLogCreateDto**](ProjectTimeLogCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project_time_log_async

> delete_project_time_log_async(tenant_id, time_log_id, api_version, x_api_version)
Delete a project time log

Deletes a project time log entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**time_log_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_period_time_logs_async

> models::ProjectTimeLogDtoListEnvelope get_project_period_time_logs_async(tenant_id, project_period_id, api_version, x_api_version)
Retrieve project period time logs

Retrieves a list of time logs for a specific project period with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**project_period_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_log_by_id_async

> models::ProjectTimeLogDtoEnvelope get_project_time_log_by_id_async(time_log_id, tenant_id, api_version, x_api_version)
Retrieve a project time log by ID

Retrieves a single project time log by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**time_log_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTimeLogDtoEnvelope**](ProjectTimeLogDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_logs_async

> models::ProjectTimeLogDtoListEnvelope get_project_time_logs_async(project_id, tenant_id, api_version, x_api_version)
Retrieve time logs for a project

Retrieves all time logs associated with the specified project.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_logs_by_responsible_contact_async

> models::ProjectTimeLogDtoListEnvelope get_project_time_logs_by_responsible_contact_async(contact_id, tenant_id, api_version, x_api_version)
Retrieve time logs by responsible contact

Retrieves time logs where the specified contact is the responsible party.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project_time_logs_created_by_contact_async

> models::ProjectTimeLogDtoListEnvelope get_project_time_logs_created_by_contact_async(contact_id, tenant_id, api_version, x_api_version)
Retrieve time logs created by a contact

Retrieves time logs that were created by the specified contact.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProjectTimeLogDtoListEnvelope**](ProjectTimeLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_time_log_async

> update_project_time_log_async(time_log_id, tenant_id, api_version, x_api_version, project_time_log_update_dto)
Update a project time log

Updates an existing project time log entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**time_log_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_time_log_update_dto** | Option<[**ProjectTimeLogUpdateDto**](ProjectTimeLogUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

