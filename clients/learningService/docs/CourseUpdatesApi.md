# \CourseUpdatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_update_async**](CourseUpdatesApi.md#create_course_update_async) | **POST** /api/v2/LearningService/CourseUpdates | Create a new course update
[**delete_course_update_async**](CourseUpdatesApi.md#delete_course_update_async) | **DELETE** /api/v2/LearningService/CourseUpdates/{updateId} | Delete a course update
[**get_course_update_by_id_async**](CourseUpdatesApi.md#get_course_update_by_id_async) | **GET** /api/v2/LearningService/CourseUpdates/{updateId} | Get course update by ID
[**get_course_updates_async**](CourseUpdatesApi.md#get_course_updates_async) | **GET** /api/v2/LearningService/CourseUpdates | Get all course updates
[**get_course_updates_count_async**](CourseUpdatesApi.md#get_course_updates_count_async) | **GET** /api/v2/LearningService/CourseUpdates/Count | Get course updates count
[**update_course_update_async**](CourseUpdatesApi.md#update_course_update_async) | **PUT** /api/v2/LearningService/CourseUpdates/{updateId} | Update a course update



## create_course_update_async

> create_course_update_async(tenant_id, api_version, x_api_version, course_news_create_dto)
Create a new course update

Creates a new course update for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_news_create_dto** | Option<[**CourseNewsCreateDto**](CourseNewsCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_update_async

> delete_course_update_async(tenant_id, update_id, api_version, x_api_version)
Delete a course update

Deletes a course update for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**update_id** | **String** |  | [required] |
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


## get_course_update_by_id_async

> models::CourseNewsDto get_course_update_by_id_async(update_id, api_version, x_api_version)
Get course update by ID

Retrieves a specific course update by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseNewsDto**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_updates_async

> Vec<models::CourseNewsDto> get_course_updates_async(tenant_id, api_version, x_api_version)
Get all course updates

Retrieves all course updates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseNewsDto>**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_updates_count_async

> i32 get_course_updates_count_async(tenant_id, api_version, x_api_version)
Get course updates count

Returns the count of course updates for the specified tenant.

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


## update_course_update_async

> update_course_update_async(tenant_id, update_id, api_version, x_api_version, course_news_update_dto)
Update a course update

Updates an existing course update for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**update_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_news_update_dto** | Option<[**CourseNewsUpdateDto**](CourseNewsUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

