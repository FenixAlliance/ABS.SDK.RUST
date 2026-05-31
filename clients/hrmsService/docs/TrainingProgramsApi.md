# \TrainingProgramsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_training_program_async**](TrainingProgramsApi.md#create_training_program_async) | **POST** /api/v2/HrmsService/TrainingPrograms | Create a training program
[**delete_training_program_async**](TrainingProgramsApi.md#delete_training_program_async) | **DELETE** /api/v2/HrmsService/TrainingPrograms/{programId} | Delete a training program
[**get_training_program_by_id_async**](TrainingProgramsApi.md#get_training_program_by_id_async) | **GET** /api/v2/HrmsService/TrainingPrograms/{programId} | Get training program by ID
[**get_training_programs_async**](TrainingProgramsApi.md#get_training_programs_async) | **GET** /api/v2/HrmsService/TrainingPrograms | Get training programs
[**get_training_programs_count_async**](TrainingProgramsApi.md#get_training_programs_count_async) | **GET** /api/v2/HrmsService/TrainingPrograms/Count | Count training programs
[**update_training_program_async**](TrainingProgramsApi.md#update_training_program_async) | **PUT** /api/v2/HrmsService/TrainingPrograms/{programId} | Update a training program



## create_training_program_async

> models::EmptyEnvelope create_training_program_async(tenant_id, api_version, x_api_version, training_program_create_dto)
Create a training program

Creates a new training program for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_create_dto** | Option<[**TrainingProgramCreateDto**](TrainingProgramCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_training_program_async

> models::EmptyEnvelope delete_training_program_async(tenant_id, program_id, api_version, x_api_version)
Delete a training program

Deletes a training program for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**program_id** | **uuid::Uuid** |  | [required] |
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


## get_training_program_by_id_async

> models::TrainingProgramDtoEnvelope get_training_program_by_id_async(tenant_id, program_id, api_version, x_api_version)
Get training program by ID

Retrieves a specific training program by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**program_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramDtoEnvelope**](TrainingProgramDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_programs_async

> models::TrainingProgramDtoListEnvelope get_training_programs_async(tenant_id, api_version, x_api_version)
Get training programs

Retrieves training programs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramDtoListEnvelope**](TrainingProgramDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_programs_count_async

> models::Int32Envelope get_training_programs_count_async(tenant_id, api_version, x_api_version)
Count training programs

Counts training programs for the specified tenant.

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


## update_training_program_async

> models::EmptyEnvelope update_training_program_async(tenant_id, program_id, api_version, x_api_version, training_program_update_dto)
Update a training program

Updates an existing training program for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**program_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_update_dto** | Option<[**TrainingProgramUpdateDto**](TrainingProgramUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

