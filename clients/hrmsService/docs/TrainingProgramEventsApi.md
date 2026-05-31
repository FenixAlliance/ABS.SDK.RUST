# \TrainingProgramEventsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_training_program_event_async**](TrainingProgramEventsApi.md#create_training_program_event_async) | **POST** /api/v2/HrmsService/TrainingProgramEvents | Create a training program event
[**delete_training_program_event_async**](TrainingProgramEventsApi.md#delete_training_program_event_async) | **DELETE** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Delete a training program event
[**get_training_program_event_by_id_async**](TrainingProgramEventsApi.md#get_training_program_event_by_id_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Get training program event by ID
[**get_training_program_events_async**](TrainingProgramEventsApi.md#get_training_program_events_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents | Get training program events
[**get_training_program_events_count_async**](TrainingProgramEventsApi.md#get_training_program_events_count_async) | **GET** /api/v2/HrmsService/TrainingProgramEvents/Count | Count training program events
[**update_training_program_event_async**](TrainingProgramEventsApi.md#update_training_program_event_async) | **PUT** /api/v2/HrmsService/TrainingProgramEvents/{eventId} | Update a training program event



## create_training_program_event_async

> models::EmptyEnvelope create_training_program_event_async(tenant_id, api_version, x_api_version, training_program_event_create_dto)
Create a training program event

Creates a new training program event for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_event_create_dto** | Option<[**TrainingProgramEventCreateDto**](TrainingProgramEventCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_training_program_event_async

> models::EmptyEnvelope delete_training_program_event_async(tenant_id, event_id, api_version, x_api_version)
Delete a training program event

Deletes a training program event for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**event_id** | **uuid::Uuid** |  | [required] |
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


## get_training_program_event_by_id_async

> models::TrainingProgramEventDtoEnvelope get_training_program_event_by_id_async(tenant_id, event_id, api_version, x_api_version)
Get training program event by ID

Retrieves a specific training program event by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**event_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramEventDtoEnvelope**](TrainingProgramEventDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_program_events_async

> models::TrainingProgramEventDtoListEnvelope get_training_program_events_async(tenant_id, api_version, x_api_version)
Get training program events

Retrieves training program events for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramEventDtoListEnvelope**](TrainingProgramEventDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_program_events_count_async

> models::Int32Envelope get_training_program_events_count_async(tenant_id, api_version, x_api_version)
Count training program events

Counts training program events for the specified tenant.

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


## update_training_program_event_async

> models::EmptyEnvelope update_training_program_event_async(tenant_id, event_id, api_version, x_api_version, training_program_event_update_dto)
Update a training program event

Updates an existing training program event for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**event_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_event_update_dto** | Option<[**TrainingProgramEventUpdateDto**](TrainingProgramEventUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

