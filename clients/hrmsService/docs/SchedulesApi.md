# \SchedulesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_schedule_async**](SchedulesApi.md#create_schedule_async) | **POST** /api/v2/HrmsService/Schedules | Create a schedule
[**delete_schedule_async**](SchedulesApi.md#delete_schedule_async) | **DELETE** /api/v2/HrmsService/Schedules/{scheduleId} | Delete a schedule
[**get_schedule_by_id_async**](SchedulesApi.md#get_schedule_by_id_async) | **GET** /api/v2/HrmsService/Schedules/{scheduleId} | Get schedule by ID
[**get_schedules_async**](SchedulesApi.md#get_schedules_async) | **GET** /api/v2/HrmsService/Schedules | Get schedules
[**get_schedules_count_async**](SchedulesApi.md#get_schedules_count_async) | **GET** /api/v2/HrmsService/Schedules/Count | Count schedules
[**update_schedule_async**](SchedulesApi.md#update_schedule_async) | **PUT** /api/v2/HrmsService/Schedules/{scheduleId} | Update a schedule



## create_schedule_async

> models::EmptyEnvelope create_schedule_async(tenant_id, api_version, x_api_version, schedule_create_dto)
Create a schedule

Creates a new schedule for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**schedule_create_dto** | Option<[**ScheduleCreateDto**](ScheduleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_schedule_async

> models::EmptyEnvelope delete_schedule_async(tenant_id, schedule_id, api_version, x_api_version)
Delete a schedule

Deletes a schedule for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**schedule_id** | **uuid::Uuid** |  | [required] |
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


## get_schedule_by_id_async

> models::ScheduleDtoEnvelope get_schedule_by_id_async(tenant_id, schedule_id, api_version, x_api_version)
Get schedule by ID

Retrieves a specific schedule by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**schedule_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ScheduleDtoEnvelope**](ScheduleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_schedules_async

> models::ScheduleDtoListEnvelope get_schedules_async(tenant_id, api_version, x_api_version)
Get schedules

Retrieves schedules for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ScheduleDtoListEnvelope**](ScheduleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_schedules_count_async

> models::Int32Envelope get_schedules_count_async(tenant_id, api_version, x_api_version)
Count schedules

Counts schedules for the specified tenant.

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


## update_schedule_async

> models::EmptyEnvelope update_schedule_async(tenant_id, schedule_id, api_version, x_api_version, schedule_update_dto)
Update a schedule

Updates an existing schedule for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**schedule_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**schedule_update_dto** | Option<[**ScheduleUpdateDto**](ScheduleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

