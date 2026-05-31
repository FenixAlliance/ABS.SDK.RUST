# \CourseEnrollmentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_enrollment_async**](CourseEnrollmentsApi.md#create_course_enrollment_async) | **POST** /api/v2/LearningService/CourseEnrollments | Create a new course enrollment
[**delete_course_enrollment_async**](CourseEnrollmentsApi.md#delete_course_enrollment_async) | **DELETE** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Delete a course enrollment
[**get_course_enrollment_async**](CourseEnrollmentsApi.md#get_course_enrollment_async) | **GET** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Get course enrollment by ID
[**get_enrollments_async**](CourseEnrollmentsApi.md#get_enrollments_async) | **GET** /api/v2/LearningService/CourseEnrollments | Get all course enrollments
[**get_enrollments_count_async**](CourseEnrollmentsApi.md#get_enrollments_count_async) | **GET** /api/v2/LearningService/CourseEnrollments/Count | Get course enrollments count
[**get_student_course_enrollments_async**](CourseEnrollmentsApi.md#get_student_course_enrollments_async) | **GET** /api/v2/LearningService/CourseEnrollments/Student/{studentProfileId} | Get enrollments by student
[**update_course_enrollment_async**](CourseEnrollmentsApi.md#update_course_enrollment_async) | **PUT** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Update a course enrollment



## create_course_enrollment_async

> create_course_enrollment_async(tenant_id, api_version, x_api_version, course_enrollment_create_dto)
Create a new course enrollment

Creates a new course enrollment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_enrollment_create_dto** | Option<[**CourseEnrollmentCreateDto**](CourseEnrollmentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_enrollment_async

> delete_course_enrollment_async(tenant_id, course_enrollment_id, api_version, x_api_version)
Delete a course enrollment

Deletes a course enrollment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_enrollment_id** | **uuid::Uuid** |  | [required] |
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


## get_course_enrollment_async

> models::CourseEnrollmentDto get_course_enrollment_async(tenant_id, course_enrollment_id, api_version, x_api_version)
Get course enrollment by ID

Retrieves a specific course enrollment by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseEnrollmentDto**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollments_async

> Vec<models::CourseEnrollmentDto> get_enrollments_async(tenant_id, api_version, x_api_version)
Get all course enrollments

Retrieves all course enrollments for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseEnrollmentDto>**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollments_count_async

> i32 get_enrollments_count_async(tenant_id, api_version, x_api_version)
Get course enrollments count

Returns the count of course enrollments for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

**i32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_student_course_enrollments_async

> Vec<models::CourseEnrollmentDto> get_student_course_enrollments_async(tenant_id, student_profile_id, api_version, x_api_version)
Get enrollments by student

Retrieves all enrollments for a specific student.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseEnrollmentDto>**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_course_enrollment_async

> update_course_enrollment_async(tenant_id, course_enrollment_id, api_version, x_api_version, course_enrollment_update_dto)
Update a course enrollment

Updates an existing course enrollment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_enrollment_update_dto** | Option<[**CourseEnrollmentUpdateDto**](CourseEnrollmentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

