# \CourseLibrariesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_library_async**](CourseLibrariesApi.md#create_course_library_async) | **POST** /api/v2/LearningService/CourseLibraries | Create a course library
[**delete_course_library_async**](CourseLibrariesApi.md#delete_course_library_async) | **DELETE** /api/v2/LearningService/CourseLibraries/{libraryId} | Delete a course library
[**get_course_libraries_async**](CourseLibrariesApi.md#get_course_libraries_async) | **GET** /api/v2/LearningService/CourseLibraries | Get all course libraries
[**get_course_libraries_count_async**](CourseLibrariesApi.md#get_course_libraries_count_async) | **GET** /api/v2/LearningService/CourseLibraries/Count | Get course libraries count
[**get_course_library_by_id_async**](CourseLibrariesApi.md#get_course_library_by_id_async) | **GET** /api/v2/LearningService/CourseLibraries/{libraryId} | Get course library by ID
[**update_course_library_async**](CourseLibrariesApi.md#update_course_library_async) | **PUT** /api/v2/LearningService/CourseLibraries/{libraryId} | Update a course library



## create_course_library_async

> models::CourseLibraryDto create_course_library_async(tenant_id, api_version, x_api_version, course_library_create_dto)
Create a course library

Creates a new course library for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_library_create_dto** | Option<[**CourseLibraryCreateDto**](CourseLibraryCreateDto.md)> |  |  |

### Return type

[**models::CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_library_async

> delete_course_library_async(tenant_id, library_id, api_version, x_api_version)
Delete a course library

Deletes a course library by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**library_id** | **String** |  | [required] |
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


## get_course_libraries_async

> Vec<models::CourseLibraryDto> get_course_libraries_async(tenant_id, api_version, x_api_version)
Get all course libraries

Retrieves all course libraries for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseLibraryDto>**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_libraries_count_async

> i32 get_course_libraries_count_async(tenant_id, api_version, x_api_version)
Get course libraries count

Returns the count of course libraries for the specified tenant.

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


## get_course_library_by_id_async

> models::CourseLibraryDto get_course_library_by_id_async(library_id, api_version, x_api_version)
Get course library by ID

Retrieves a specific course library by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**library_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_course_library_async

> models::CourseLibraryDto update_course_library_async(tenant_id, library_id, api_version, x_api_version, course_library_update_dto)
Update a course library

Updates an existing course library.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**library_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_library_update_dto** | Option<[**CourseLibraryUpdateDto**](CourseLibraryUpdateDto.md)> |  |  |

### Return type

[**models::CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

