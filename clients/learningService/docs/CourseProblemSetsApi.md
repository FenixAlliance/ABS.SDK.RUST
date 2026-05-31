# \CourseProblemSetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_problem_set_async**](CourseProblemSetsApi.md#create_course_problem_set_async) | **POST** /api/v2/LearningService/CourseProblemSets | Create a new course problem set
[**delete_course_problem_set_async**](CourseProblemSetsApi.md#delete_course_problem_set_async) | **DELETE** /api/v2/LearningService/CourseProblemSets/{problemSetId} | Delete a course problem set
[**get_course_problem_set_by_id_async**](CourseProblemSetsApi.md#get_course_problem_set_by_id_async) | **GET** /api/v2/LearningService/CourseProblemSets/{problemSetId} | Get course problem set by ID
[**get_course_problem_sets_async**](CourseProblemSetsApi.md#get_course_problem_sets_async) | **GET** /api/v2/LearningService/CourseProblemSets | Get all course problem sets
[**get_course_problem_sets_count_async**](CourseProblemSetsApi.md#get_course_problem_sets_count_async) | **GET** /api/v2/LearningService/CourseProblemSets/Count | Get course problem sets count
[**update_course_problem_set_async**](CourseProblemSetsApi.md#update_course_problem_set_async) | **PUT** /api/v2/LearningService/CourseProblemSets/{problemSetId} | Update a course problem set



## create_course_problem_set_async

> create_course_problem_set_async(tenant_id, api_version, x_api_version, course_problem_set_create_dto)
Create a new course problem set

Creates a new course problem set for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_problem_set_create_dto** | Option<[**CourseProblemSetCreateDto**](CourseProblemSetCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_problem_set_async

> delete_course_problem_set_async(tenant_id, problem_set_id, api_version, x_api_version)
Delete a course problem set

Deletes a course problem set for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**problem_set_id** | **String** |  | [required] |
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


## get_course_problem_set_by_id_async

> models::CourseProblemSetDto get_course_problem_set_by_id_async(problem_set_id, api_version, x_api_version)
Get course problem set by ID

Retrieves a specific course problem set by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**problem_set_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseProblemSetDto**](CourseProblemSetDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_problem_sets_async

> Vec<models::CourseProblemSetDto> get_course_problem_sets_async(tenant_id, api_version, x_api_version)
Get all course problem sets

Retrieves all course problem sets for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseProblemSetDto>**](CourseProblemSetDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_problem_sets_count_async

> i32 get_course_problem_sets_count_async(tenant_id, api_version, x_api_version)
Get course problem sets count

Returns the count of course problem sets for the specified tenant.

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


## update_course_problem_set_async

> update_course_problem_set_async(tenant_id, problem_set_id, api_version, x_api_version, course_problem_set_update_dto)
Update a course problem set

Updates an existing course problem set for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**problem_set_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_problem_set_update_dto** | Option<[**CourseProblemSetUpdateDto**](CourseProblemSetUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

