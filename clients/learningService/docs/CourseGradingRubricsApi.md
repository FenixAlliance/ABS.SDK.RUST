# \CourseGradingRubricsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_grading_rubric_async**](CourseGradingRubricsApi.md#create_course_grading_rubric_async) | **POST** /api/v2/LearningService/CourseGradingRubrics | Create a course grading rubric
[**delete_course_grading_rubric_async**](CourseGradingRubricsApi.md#delete_course_grading_rubric_async) | **DELETE** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Delete a course grading rubric
[**get_course_grading_rubric_by_id_async**](CourseGradingRubricsApi.md#get_course_grading_rubric_by_id_async) | **GET** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Get course grading rubric by ID
[**get_course_grading_rubrics_async**](CourseGradingRubricsApi.md#get_course_grading_rubrics_async) | **GET** /api/v2/LearningService/CourseGradingRubrics | Get all course grading rubrics
[**get_course_grading_rubrics_count_async**](CourseGradingRubricsApi.md#get_course_grading_rubrics_count_async) | **GET** /api/v2/LearningService/CourseGradingRubrics/Count | Get course grading rubrics count
[**update_course_grading_rubric_async**](CourseGradingRubricsApi.md#update_course_grading_rubric_async) | **PUT** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Update a course grading rubric



## create_course_grading_rubric_async

> create_course_grading_rubric_async(tenant_id, api_version, x_api_version, course_grading_rubric_create_dto)
Create a course grading rubric

Creates a new course grading rubric for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_grading_rubric_create_dto** | Option<[**CourseGradingRubricCreateDto**](CourseGradingRubricCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_grading_rubric_async

> delete_course_grading_rubric_async(tenant_id, rubric_id, api_version, x_api_version)
Delete a course grading rubric

Deletes a course grading rubric by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rubric_id** | **String** |  | [required] |
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


## get_course_grading_rubric_by_id_async

> models::CourseGradingRubricDto get_course_grading_rubric_by_id_async(rubric_id, api_version, x_api_version)
Get course grading rubric by ID

Retrieves a specific course grading rubric by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**rubric_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseGradingRubricDto**](CourseGradingRubricDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_grading_rubrics_async

> Vec<models::CourseGradingRubricDto> get_course_grading_rubrics_async(tenant_id, api_version, x_api_version)
Get all course grading rubrics

Retrieves all course grading rubrics for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseGradingRubricDto>**](CourseGradingRubricDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_grading_rubrics_count_async

> i32 get_course_grading_rubrics_count_async(tenant_id, api_version, x_api_version)
Get course grading rubrics count

Returns the count of course grading rubrics for the specified tenant.

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


## update_course_grading_rubric_async

> update_course_grading_rubric_async(tenant_id, rubric_id, api_version, x_api_version, course_grading_rubric_update_dto)
Update a course grading rubric

Updates an existing course grading rubric.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rubric_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_grading_rubric_update_dto** | Option<[**CourseGradingRubricUpdateDto**](CourseGradingRubricUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

