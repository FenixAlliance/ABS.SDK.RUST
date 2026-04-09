# \CourseHandoutsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_handout_async**](CourseHandoutsApi.md#create_course_handout_async) | **POST** /api/v2/LearningService/CourseHandouts | Create a course handout
[**delete_course_handout_async**](CourseHandoutsApi.md#delete_course_handout_async) | **DELETE** /api/v2/LearningService/CourseHandouts/{handoutId} | Delete a course handout
[**get_course_handout_by_id_async**](CourseHandoutsApi.md#get_course_handout_by_id_async) | **GET** /api/v2/LearningService/CourseHandouts/{handoutId} | Get course handout by ID
[**get_course_handouts_async**](CourseHandoutsApi.md#get_course_handouts_async) | **GET** /api/v2/LearningService/CourseHandouts | Get all course handouts
[**get_course_handouts_count_async**](CourseHandoutsApi.md#get_course_handouts_count_async) | **GET** /api/v2/LearningService/CourseHandouts/Count | Get course handouts count
[**update_course_handout_async**](CourseHandoutsApi.md#update_course_handout_async) | **PUT** /api/v2/LearningService/CourseHandouts/{handoutId} | Update a course handout



## create_course_handout_async

> models::CourseHandoutDto create_course_handout_async(tenant_id, api_version, x_api_version, course_handout_create_dto)
Create a course handout

Creates a new course handout for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_handout_create_dto** | Option<[**CourseHandoutCreateDto**](CourseHandoutCreateDto.md)> |  |  |

### Return type

[**models::CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_handout_async

> delete_course_handout_async(tenant_id, handout_id, api_version, x_api_version)
Delete a course handout

Deletes a course handout by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**handout_id** | **String** |  | [required] |
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


## get_course_handout_by_id_async

> models::CourseHandoutDto get_course_handout_by_id_async(handout_id, api_version, x_api_version)
Get course handout by ID

Retrieves a specific course handout by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**handout_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_handouts_async

> Vec<models::CourseHandoutDto> get_course_handouts_async(tenant_id, api_version, x_api_version)
Get all course handouts

Retrieves all course handouts for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseHandoutDto>**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_handouts_count_async

> i32 get_course_handouts_count_async(tenant_id, api_version, x_api_version)
Get course handouts count

Returns the count of course handouts for the specified tenant.

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


## update_course_handout_async

> models::CourseHandoutDto update_course_handout_async(tenant_id, handout_id, api_version, x_api_version, course_handout_update_dto)
Update a course handout

Updates an existing course handout.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**handout_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_handout_update_dto** | Option<[**CourseHandoutUpdateDto**](CourseHandoutUpdateDto.md)> |  |  |

### Return type

[**models::CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

