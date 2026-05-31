# \CourseContentGroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_content_group_async**](CourseContentGroupsApi.md#create_course_content_group_async) | **POST** /api/v2/LearningService/CourseContentGroups | Create a new course content group
[**delete_course_content_group_async**](CourseContentGroupsApi.md#delete_course_content_group_async) | **DELETE** /api/v2/LearningService/CourseContentGroups/{groupId} | Delete a course content group
[**get_course_content_group_by_id_async**](CourseContentGroupsApi.md#get_course_content_group_by_id_async) | **GET** /api/v2/LearningService/CourseContentGroups/{groupId} | Get course content group by ID
[**get_course_content_groups_async**](CourseContentGroupsApi.md#get_course_content_groups_async) | **GET** /api/v2/LearningService/CourseContentGroups | Get all course content groups
[**get_course_content_groups_by_course_async**](CourseContentGroupsApi.md#get_course_content_groups_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ContentGroups | Get course content groups by course
[**get_course_content_groups_by_course_count_async**](CourseContentGroupsApi.md#get_course_content_groups_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ContentGroups/Count | Get course content groups count by course
[**get_course_content_groups_count_async**](CourseContentGroupsApi.md#get_course_content_groups_count_async) | **GET** /api/v2/LearningService/CourseContentGroups/Count | Get course content groups count
[**update_course_content_group_async**](CourseContentGroupsApi.md#update_course_content_group_async) | **PUT** /api/v2/LearningService/CourseContentGroups/{groupId} | Update a course content group



## create_course_content_group_async

> create_course_content_group_async(tenant_id, api_version, x_api_version, course_content_group_create_dto)
Create a new course content group

Creates a new course content group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_content_group_create_dto** | Option<[**CourseContentGroupCreateDto**](CourseContentGroupCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_content_group_async

> delete_course_content_group_async(tenant_id, group_id, api_version, x_api_version)
Delete a course content group

Deletes a course content group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**group_id** | **String** |  | [required] |
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


## get_course_content_group_by_id_async

> models::CourseContentGroupDto get_course_content_group_by_id_async(group_id, api_version, x_api_version)
Get course content group by ID

Retrieves a specific course content group by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**group_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseContentGroupDto**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_content_groups_async

> Vec<models::CourseContentGroupDto> get_course_content_groups_async(tenant_id, api_version, x_api_version)
Get all course content groups

Retrieves all course content groups for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseContentGroupDto>**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_content_groups_by_course_async

> Vec<models::CourseContentGroupDto> get_course_content_groups_by_course_async(course_id, api_version, x_api_version)
Get course content groups by course

Retrieves all course content groups for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseContentGroupDto>**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_content_groups_by_course_count_async

> i32 get_course_content_groups_by_course_count_async(course_id, api_version, x_api_version)
Get course content groups count by course

Returns the count of course content groups for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_content_groups_count_async

> i32 get_course_content_groups_count_async(tenant_id, api_version, x_api_version)
Get course content groups count

Returns the count of course content groups for the specified tenant.

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


## update_course_content_group_async

> update_course_content_group_async(tenant_id, group_id, api_version, x_api_version, course_content_group_update_dto)
Update a course content group

Updates an existing course content group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**group_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_content_group_update_dto** | Option<[**CourseContentGroupUpdateDto**](CourseContentGroupUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

