# \CourseAssignmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_assignment_async**](CourseAssignmentsApi.md#create_course_assignment_async) | **POST** /api/v2/LearningService/CourseAssignments | Create a new course assignment
[**delete_course_assignment_async**](CourseAssignmentsApi.md#delete_course_assignment_async) | **DELETE** /api/v2/LearningService/CourseAssignments/{assignmentId} | Delete a course assignment
[**get_course_assignment_by_id_async**](CourseAssignmentsApi.md#get_course_assignment_by_id_async) | **GET** /api/v2/LearningService/CourseAssignments/{assignmentId} | Get course assignment by ID
[**get_course_assignments_async**](CourseAssignmentsApi.md#get_course_assignments_async) | **GET** /api/v2/LearningService/CourseAssignments | Get all course assignments
[**get_course_assignments_count_async**](CourseAssignmentsApi.md#get_course_assignments_count_async) | **GET** /api/v2/LearningService/CourseAssignments/Count | Get course assignments count
[**update_course_assignment_async**](CourseAssignmentsApi.md#update_course_assignment_async) | **PUT** /api/v2/LearningService/CourseAssignments/{assignmentId} | Update a course assignment



## create_course_assignment_async

> create_course_assignment_async(tenant_id, api_version, x_api_version, course_assignment_create_dto)
Create a new course assignment

Creates a new course assignment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_create_dto** | Option<[**CourseAssignmentCreateDto**](CourseAssignmentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_assignment_async

> delete_course_assignment_async(tenant_id, assignment_id, api_version, x_api_version)
Delete a course assignment

Deletes a course assignment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**assignment_id** | **String** |  | [required] |
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


## get_course_assignment_by_id_async

> models::CourseAssignmentDto get_course_assignment_by_id_async(assignment_id, api_version, x_api_version)
Get course assignment by ID

Retrieves a specific course assignment by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**assignment_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseAssignmentDto**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignments_async

> Vec<models::CourseAssignmentDto> get_course_assignments_async(tenant_id, api_version, x_api_version)
Get all course assignments

Retrieves all course assignments for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseAssignmentDto>**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignments_count_async

> i32 get_course_assignments_count_async(tenant_id, api_version, x_api_version)
Get course assignments count

Returns the count of course assignments for the specified tenant.

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


## update_course_assignment_async

> update_course_assignment_async(tenant_id, assignment_id, api_version, x_api_version, course_assignment_update_dto)
Update a course assignment

Updates an existing course assignment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**assignment_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_update_dto** | Option<[**CourseAssignmentUpdateDto**](CourseAssignmentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

