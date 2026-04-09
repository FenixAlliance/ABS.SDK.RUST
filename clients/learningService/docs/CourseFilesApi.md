# \CourseFilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_file_async**](CourseFilesApi.md#create_course_file_async) | **POST** /api/v2/LearningService/CourseFiles | Create a new course file
[**delete_course_file_async**](CourseFilesApi.md#delete_course_file_async) | **DELETE** /api/v2/LearningService/CourseFiles/{fileId} | Delete a course file
[**get_course_file_by_id_async**](CourseFilesApi.md#get_course_file_by_id_async) | **GET** /api/v2/LearningService/CourseFiles/{fileId} | Get course file by ID
[**get_course_files_async**](CourseFilesApi.md#get_course_files_async) | **GET** /api/v2/LearningService/CourseFiles | Get all course files
[**get_course_files_count_async**](CourseFilesApi.md#get_course_files_count_async) | **GET** /api/v2/LearningService/CourseFiles/Count | Get course files count
[**update_course_file_async**](CourseFilesApi.md#update_course_file_async) | **PUT** /api/v2/LearningService/CourseFiles/{fileId} | Update a course file



## create_course_file_async

> create_course_file_async(tenant_id, api_version, x_api_version, course_file_create_dto)
Create a new course file

Creates a new course file for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_file_create_dto** | Option<[**CourseFileCreateDto**](CourseFileCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_file_async

> delete_course_file_async(tenant_id, file_id, api_version, x_api_version)
Delete a course file

Deletes a course file for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**file_id** | **String** |  | [required] |
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


## get_course_file_by_id_async

> models::CourseFileDto get_course_file_by_id_async(file_id, api_version, x_api_version)
Get course file by ID

Retrieves a specific course file by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseFileDto**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_files_async

> Vec<models::CourseFileDto> get_course_files_async(tenant_id, api_version, x_api_version)
Get all course files

Retrieves all course files for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseFileDto>**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_files_count_async

> i32 get_course_files_count_async(tenant_id, api_version, x_api_version)
Get course files count

Returns the count of course files for the specified tenant.

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


## update_course_file_async

> update_course_file_async(tenant_id, file_id, api_version, x_api_version, course_file_update_dto)
Update a course file

Updates an existing course file for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**file_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_file_update_dto** | Option<[**CourseFileUpdateDto**](CourseFileUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

