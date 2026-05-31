# \CoursePagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_page_async**](CoursePagesApi.md#create_course_page_async) | **POST** /api/v2/LearningService/CoursePages | Create a new course page
[**delete_course_page_async**](CoursePagesApi.md#delete_course_page_async) | **DELETE** /api/v2/LearningService/CoursePages/{pageId} | Delete a course page
[**get_course_page_by_id_async**](CoursePagesApi.md#get_course_page_by_id_async) | **GET** /api/v2/LearningService/CoursePages/{pageId} | Get course page by ID
[**get_course_pages_async**](CoursePagesApi.md#get_course_pages_async) | **GET** /api/v2/LearningService/CoursePages | Get all course pages
[**get_course_pages_count_async**](CoursePagesApi.md#get_course_pages_count_async) | **GET** /api/v2/LearningService/CoursePages/Count | Get course pages count
[**update_course_page_async**](CoursePagesApi.md#update_course_page_async) | **PUT** /api/v2/LearningService/CoursePages/{pageId} | Update a course page



## create_course_page_async

> create_course_page_async(tenant_id, api_version, x_api_version, course_page_create_dto)
Create a new course page

Creates a new course page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_page_create_dto** | Option<[**CoursePageCreateDto**](CoursePageCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_page_async

> delete_course_page_async(tenant_id, page_id, api_version, x_api_version)
Delete a course page

Deletes a course page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**page_id** | **String** |  | [required] |
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


## get_course_page_by_id_async

> models::CoursePageDto get_course_page_by_id_async(page_id, api_version, x_api_version)
Get course page by ID

Retrieves a specific course page by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**page_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CoursePageDto**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_pages_async

> Vec<models::CoursePageDto> get_course_pages_async(tenant_id, api_version, x_api_version)
Get all course pages

Retrieves all course pages for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CoursePageDto>**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_pages_count_async

> i32 get_course_pages_count_async(tenant_id, api_version, x_api_version)
Get course pages count

Returns the count of course pages for the specified tenant.

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


## update_course_page_async

> update_course_page_async(tenant_id, page_id, api_version, x_api_version, course_page_update_dto)
Update a course page

Updates an existing course page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**page_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_page_update_dto** | Option<[**CoursePageUpdateDto**](CoursePageUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

