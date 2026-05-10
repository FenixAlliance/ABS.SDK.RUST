# \MeApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_my_average_score_async**](MeApi.md#get_my_average_score_async) | **GET** /api/v2/LearningService/Me/AverageScore | Get current user's average score
[**get_my_certificates_async**](MeApi.md#get_my_certificates_async) | **GET** /api/v2/LearningService/Me/Certificates | Get current user's completion certificates
[**get_my_certificates_count_async**](MeApi.md#get_my_certificates_count_async) | **GET** /api/v2/LearningService/Me/Certificates/Count | Get current user's certificates count
[**get_my_enrollments_async**](MeApi.md#get_my_enrollments_async) | **GET** /api/v2/LearningService/Me/Enrollments | Get current user's course enrollments
[**get_my_enrollments_count_async**](MeApi.md#get_my_enrollments_count_async) | **GET** /api/v2/LearningService/Me/Enrollments/Count | Get current user's enrollment count
[**get_my_hours_completed_async**](MeApi.md#get_my_hours_completed_async) | **GET** /api/v2/LearningService/Me/HoursCompleted | Get current user's completed hours
[**get_my_instructor_courses_async**](MeApi.md#get_my_instructor_courses_async) | **GET** /api/v2/LearningService/Me/InstructorCourses | Get current user's instructor courses
[**get_my_instructor_courses_count_async**](MeApi.md#get_my_instructor_courses_count_async) | **GET** /api/v2/LearningService/Me/InstructorCourses/Count | Get current user's instructor courses count
[**get_my_instructor_profiles_async**](MeApi.md#get_my_instructor_profiles_async) | **GET** /api/v2/LearningService/Me/InstructorProfiles | Get current user's instructor profiles
[**get_my_instructor_profiles_count_async**](MeApi.md#get_my_instructor_profiles_count_async) | **GET** /api/v2/LearningService/Me/InstructorProfiles/Count | Get current user's instructor profiles count
[**get_my_pending_task_count_async**](MeApi.md#get_my_pending_task_count_async) | **GET** /api/v2/LearningService/Me/PendingTasks | Get current user's pending task count
[**get_my_student_courses_async**](MeApi.md#get_my_student_courses_async) | **GET** /api/v2/LearningService/Me/Courses | Get current user's enrolled courses
[**get_my_student_courses_count_async**](MeApi.md#get_my_student_courses_count_async) | **GET** /api/v2/LearningService/Me/Courses/Count | Get current user's enrolled courses count
[**get_my_student_profiles_async**](MeApi.md#get_my_student_profiles_async) | **GET** /api/v2/LearningService/Me/StudentProfiles | Get current user's student profiles
[**get_my_student_profiles_count_async**](MeApi.md#get_my_student_profiles_count_async) | **GET** /api/v2/LearningService/Me/StudentProfiles/Count | Get current user's student profiles count



## get_my_average_score_async

> models::AverageDtoEnvelope get_my_average_score_async(api_version, x_api_version)
Get current user's average score

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AverageDtoEnvelope**](AverageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_certificates_async

> models::CourseCompletionCertificateDtoIReadOnlyListEnvelope get_my_certificates_async(api_version, x_api_version)
Get current user's completion certificates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseCompletionCertificateDtoIReadOnlyListEnvelope**](CourseCompletionCertificateDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_certificates_count_async

> i32 get_my_certificates_count_async(api_version, x_api_version)
Get current user's certificates count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_my_enrollments_async

> models::CourseEnrollmentDtoIReadOnlyListEnvelope get_my_enrollments_async(api_version, x_api_version)
Get current user's course enrollments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseEnrollmentDtoIReadOnlyListEnvelope**](CourseEnrollmentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_enrollments_count_async

> i32 get_my_enrollments_count_async(api_version, x_api_version)
Get current user's enrollment count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_my_hours_completed_async

> models::CountDtoEnvelope get_my_hours_completed_async(api_version, x_api_version)
Get current user's completed hours

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountDtoEnvelope**](CountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_instructor_courses_async

> models::CourseDtoIReadOnlyListEnvelope get_my_instructor_courses_async(api_version, x_api_version)
Get current user's instructor courses

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseDtoIReadOnlyListEnvelope**](CourseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_instructor_courses_count_async

> i32 get_my_instructor_courses_count_async(api_version, x_api_version)
Get current user's instructor courses count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_my_instructor_profiles_async

> models::InstructorProfileDtoIReadOnlyListEnvelope get_my_instructor_profiles_async(api_version, x_api_version)
Get current user's instructor profiles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InstructorProfileDtoIReadOnlyListEnvelope**](InstructorProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_instructor_profiles_count_async

> i32 get_my_instructor_profiles_count_async(api_version, x_api_version)
Get current user's instructor profiles count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_my_pending_task_count_async

> models::CountDtoEnvelope get_my_pending_task_count_async(api_version, x_api_version)
Get current user's pending task count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountDtoEnvelope**](CountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_student_courses_async

> models::CourseDtoIReadOnlyListEnvelope get_my_student_courses_async(api_version, x_api_version)
Get current user's enrolled courses

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseDtoIReadOnlyListEnvelope**](CourseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_student_courses_count_async

> i32 get_my_student_courses_count_async(api_version, x_api_version)
Get current user's enrolled courses count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_my_student_profiles_async

> models::StudentProfileDtoIReadOnlyListEnvelope get_my_student_profiles_async(api_version, x_api_version)
Get current user's student profiles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::StudentProfileDtoIReadOnlyListEnvelope**](StudentProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_my_student_profiles_count_async

> i32 get_my_student_profiles_count_async(api_version, x_api_version)
Get current user's student profiles count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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

