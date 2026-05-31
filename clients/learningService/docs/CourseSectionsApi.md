# \CourseSectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_section_async**](CourseSectionsApi.md#create_course_section_async) | **POST** /api/v2/LearningService/CourseSections | Create a new course section
[**delete_course_section_async**](CourseSectionsApi.md#delete_course_section_async) | **DELETE** /api/v2/LearningService/CourseSections/{sectionId} | Delete a course section
[**get_course_section_by_id_async**](CourseSectionsApi.md#get_course_section_by_id_async) | **GET** /api/v2/LearningService/CourseSections/{sectionId} | Get course section by ID
[**get_course_sections_async**](CourseSectionsApi.md#get_course_sections_async) | **GET** /api/v2/LearningService/CourseSections | Get all course sections
[**get_course_sections_count_async**](CourseSectionsApi.md#get_course_sections_count_async) | **GET** /api/v2/LearningService/CourseSections/Count | Get course sections count
[**update_course_section_async**](CourseSectionsApi.md#update_course_section_async) | **PUT** /api/v2/LearningService/CourseSections/{sectionId} | Update a course section



## create_course_section_async

> create_course_section_async(tenant_id, api_version, x_api_version, course_section_create_dto)
Create a new course section

Creates a new course section for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_section_create_dto** | Option<[**CourseSectionCreateDto**](CourseSectionCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_section_async

> delete_course_section_async(tenant_id, section_id, api_version, x_api_version)
Delete a course section

Deletes a course section for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**section_id** | **String** |  | [required] |
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


## get_course_section_by_id_async

> models::CourseSectionDto get_course_section_by_id_async(section_id, api_version, x_api_version)
Get course section by ID

Retrieves a specific course section by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**section_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseSectionDto**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_sections_async

> Vec<models::CourseSectionDto> get_course_sections_async(tenant_id, api_version, x_api_version)
Get all course sections

Retrieves all course sections for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseSectionDto>**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_sections_count_async

> i32 get_course_sections_count_async(tenant_id, api_version, x_api_version)
Get course sections count

Returns the count of course sections for the specified tenant.

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


## update_course_section_async

> update_course_section_async(tenant_id, section_id, api_version, x_api_version, course_section_update_dto)
Update a course section

Updates an existing course section for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**section_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_section_update_dto** | Option<[**CourseSectionUpdateDto**](CourseSectionUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

