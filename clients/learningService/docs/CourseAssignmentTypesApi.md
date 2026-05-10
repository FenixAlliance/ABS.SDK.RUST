# \CourseAssignmentTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_assignment_type_async**](CourseAssignmentTypesApi.md#create_course_assignment_type_async) | **POST** /api/v2/LearningService/CourseAssignmentTypes | Create a course assignment type
[**delete_course_assignment_type_async**](CourseAssignmentTypesApi.md#delete_course_assignment_type_async) | **DELETE** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Delete a course assignment type
[**get_course_assignment_type_by_id_async**](CourseAssignmentTypesApi.md#get_course_assignment_type_by_id_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Get course assignment type by ID
[**get_course_assignment_types_async**](CourseAssignmentTypesApi.md#get_course_assignment_types_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes | Get all course assignment types
[**get_course_assignment_types_count_async**](CourseAssignmentTypesApi.md#get_course_assignment_types_count_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes/Count | Get course assignment types count
[**update_course_assignment_type_async**](CourseAssignmentTypesApi.md#update_course_assignment_type_async) | **PUT** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Update a course assignment type



## create_course_assignment_type_async

> create_course_assignment_type_async(tenant_id, api_version, x_api_version, course_assignment_type_create_dto)
Create a course assignment type

Creates a new course assignment type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_type_create_dto** | Option<[**CourseAssignmentTypeCreateDto**](CourseAssignmentTypeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_assignment_type_async

> delete_course_assignment_type_async(tenant_id, assignment_type_id, api_version, x_api_version)
Delete a course assignment type

Deletes a course assignment type by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**assignment_type_id** | **String** |  | [required] |
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


## get_course_assignment_type_by_id_async

> models::CourseAssignmentTypeDto get_course_assignment_type_by_id_async(assignment_type_id, api_version, x_api_version)
Get course assignment type by ID

Retrieves a specific course assignment type by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**assignment_type_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseAssignmentTypeDto**](CourseAssignmentTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignment_types_async

> Vec<models::CourseAssignmentTypeDto> get_course_assignment_types_async(tenant_id, api_version, x_api_version)
Get all course assignment types

Retrieves all course assignment types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseAssignmentTypeDto>**](CourseAssignmentTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignment_types_count_async

> i32 get_course_assignment_types_count_async(tenant_id, api_version, x_api_version)
Get course assignment types count

Returns the count of course assignment types for the specified tenant.

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


## update_course_assignment_type_async

> update_course_assignment_type_async(tenant_id, assignment_type_id, api_version, x_api_version, course_assignment_type_update_dto)
Update a course assignment type

Updates an existing course assignment type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**assignment_type_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_type_update_dto** | Option<[**CourseAssignmentTypeUpdateDto**](CourseAssignmentTypeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

