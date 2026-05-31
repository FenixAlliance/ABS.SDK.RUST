# \TrainingProgramCoursesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_training_program_course_async**](TrainingProgramCoursesApi.md#create_training_program_course_async) | **POST** /api/v2/HrmsService/TrainingProgramCourses | Create a training program course
[**delete_training_program_course_async**](TrainingProgramCoursesApi.md#delete_training_program_course_async) | **DELETE** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Delete a training program course
[**get_training_program_course_by_id_async**](TrainingProgramCoursesApi.md#get_training_program_course_by_id_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Get training program course by ID
[**get_training_program_courses_async**](TrainingProgramCoursesApi.md#get_training_program_courses_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses | Get training program courses
[**get_training_program_courses_count_async**](TrainingProgramCoursesApi.md#get_training_program_courses_count_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses/Count | Count training program courses
[**update_training_program_course_async**](TrainingProgramCoursesApi.md#update_training_program_course_async) | **PUT** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Update a training program course



## create_training_program_course_async

> models::EmptyEnvelope create_training_program_course_async(tenant_id, api_version, x_api_version, training_program_course_create_dto)
Create a training program course

Creates a new training program course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_course_create_dto** | Option<[**TrainingProgramCourseCreateDto**](TrainingProgramCourseCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_training_program_course_async

> models::EmptyEnvelope delete_training_program_course_async(tenant_id, course_id, api_version, x_api_version)
Delete a training program course

Deletes a training program course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
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


## get_training_program_course_by_id_async

> models::TrainingProgramCourseDtoEnvelope get_training_program_course_by_id_async(tenant_id, course_id, api_version, x_api_version)
Get training program course by ID

Retrieves a specific training program course by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramCourseDtoEnvelope**](TrainingProgramCourseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_program_courses_async

> models::TrainingProgramCourseDtoListEnvelope get_training_program_courses_async(tenant_id, api_version, x_api_version)
Get training program courses

Retrieves training program courses for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrainingProgramCourseDtoListEnvelope**](TrainingProgramCourseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_training_program_courses_count_async

> models::Int32Envelope get_training_program_courses_count_async(tenant_id, api_version, x_api_version)
Count training program courses

Counts training program courses for the specified tenant.

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


## update_training_program_course_async

> models::EmptyEnvelope update_training_program_course_async(tenant_id, course_id, api_version, x_api_version, training_program_course_update_dto)
Update a training program course

Updates an existing training program course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**training_program_course_update_dto** | Option<[**TrainingProgramCourseUpdateDto**](TrainingProgramCourseUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

