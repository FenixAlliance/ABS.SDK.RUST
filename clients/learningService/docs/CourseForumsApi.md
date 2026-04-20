# \CourseForumsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_forum_async**](CourseForumsApi.md#create_course_forum_async) | **POST** /api/v2/LearningService/CourseForums | Create a course forum
[**delete_course_forum_async**](CourseForumsApi.md#delete_course_forum_async) | **DELETE** /api/v2/LearningService/CourseForums/{forumId} | Delete a course forum
[**get_course_forum_by_id_async**](CourseForumsApi.md#get_course_forum_by_id_async) | **GET** /api/v2/LearningService/CourseForums/{forumId} | Get course forum by ID
[**get_course_forums_async**](CourseForumsApi.md#get_course_forums_async) | **GET** /api/v2/LearningService/CourseForums | Get all course forums
[**get_course_forums_count_async**](CourseForumsApi.md#get_course_forums_count_async) | **GET** /api/v2/LearningService/CourseForums/Count | Get course forums count
[**update_course_forum_async**](CourseForumsApi.md#update_course_forum_async) | **PUT** /api/v2/LearningService/CourseForums/{forumId} | Update a course forum



## create_course_forum_async

> models::CourseForumDto create_course_forum_async(tenant_id, api_version, x_api_version, course_forum_create_dto)
Create a course forum

Creates a new course forum for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_forum_create_dto** | Option<[**CourseForumCreateDto**](CourseForumCreateDto.md)> |  |  |

### Return type

[**models::CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_forum_async

> delete_course_forum_async(tenant_id, forum_id, api_version, x_api_version)
Delete a course forum

Deletes a course forum by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**forum_id** | **String** |  | [required] |
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


## get_course_forum_by_id_async

> models::CourseForumDto get_course_forum_by_id_async(forum_id, api_version, x_api_version)
Get course forum by ID

Retrieves a specific course forum by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**forum_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_forums_async

> Vec<models::CourseForumDto> get_course_forums_async(tenant_id, api_version, x_api_version)
Get all course forums

Retrieves all course forums for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseForumDto>**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_forums_count_async

> i32 get_course_forums_count_async(tenant_id, api_version, x_api_version)
Get course forums count

Returns the count of course forums for the specified tenant.

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


## update_course_forum_async

> models::CourseForumDto update_course_forum_async(tenant_id, forum_id, api_version, x_api_version, course_forum_update_dto)
Update a course forum

Updates an existing course forum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**forum_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_forum_update_dto** | Option<[**CourseForumUpdateDto**](CourseForumUpdateDto.md)> |  |  |

### Return type

[**models::CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

