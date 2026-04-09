# \CourseCohortsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_cohort_async**](CourseCohortsApi.md#create_course_cohort_async) | **POST** /api/v2/LearningService/CourseCohorts | Create a new course cohort
[**delete_course_cohort_async**](CourseCohortsApi.md#delete_course_cohort_async) | **DELETE** /api/v2/LearningService/CourseCohorts/{cohortId} | Delete a course cohort
[**get_course_cohort_by_id_async**](CourseCohortsApi.md#get_course_cohort_by_id_async) | **GET** /api/v2/LearningService/CourseCohorts/{cohortId} | Get course cohort by ID
[**get_course_cohorts_async**](CourseCohortsApi.md#get_course_cohorts_async) | **GET** /api/v2/LearningService/CourseCohorts | Get all course cohorts
[**get_course_cohorts_count_async**](CourseCohortsApi.md#get_course_cohorts_count_async) | **GET** /api/v2/LearningService/CourseCohorts/Count | Get course cohorts count
[**update_course_cohort_async**](CourseCohortsApi.md#update_course_cohort_async) | **PUT** /api/v2/LearningService/CourseCohorts/{cohortId} | Update a course cohort



## create_course_cohort_async

> create_course_cohort_async(tenant_id, api_version, x_api_version, course_cohort_create_dto)
Create a new course cohort

Creates a new course cohort for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_cohort_create_dto** | Option<[**CourseCohortCreateDto**](CourseCohortCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_cohort_async

> delete_course_cohort_async(tenant_id, cohort_id, api_version, x_api_version)
Delete a course cohort

Deletes a course cohort for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cohort_id** | **String** |  | [required] |
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


## get_course_cohort_by_id_async

> models::CourseCohortDto get_course_cohort_by_id_async(cohort_id, api_version, x_api_version)
Get course cohort by ID

Retrieves a specific course cohort by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cohort_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseCohortDto**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_cohorts_async

> Vec<models::CourseCohortDto> get_course_cohorts_async(tenant_id, api_version, x_api_version)
Get all course cohorts

Retrieves all course cohorts for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseCohortDto>**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_cohorts_count_async

> i32 get_course_cohorts_count_async(tenant_id, api_version, x_api_version)
Get course cohorts count

Returns the count of course cohorts for the specified tenant.

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


## update_course_cohort_async

> update_course_cohort_async(tenant_id, cohort_id, api_version, x_api_version, course_cohort_update_dto)
Update a course cohort

Updates an existing course cohort for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cohort_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_cohort_update_dto** | Option<[**CourseCohortUpdateDto**](CourseCohortUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

