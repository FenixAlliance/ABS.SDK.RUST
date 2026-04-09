# \CourseWikisApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_wiki_async**](CourseWikisApi.md#create_course_wiki_async) | **POST** /api/v2/LearningService/CourseWikis | Create a new course wiki
[**delete_course_wiki_async**](CourseWikisApi.md#delete_course_wiki_async) | **DELETE** /api/v2/LearningService/CourseWikis/{wikiId} | Delete a course wiki
[**get_course_wiki_by_id_async**](CourseWikisApi.md#get_course_wiki_by_id_async) | **GET** /api/v2/LearningService/CourseWikis/{wikiId} | Get course wiki by ID
[**get_course_wikis_async**](CourseWikisApi.md#get_course_wikis_async) | **GET** /api/v2/LearningService/CourseWikis | Get all course wikis
[**get_course_wikis_count_async**](CourseWikisApi.md#get_course_wikis_count_async) | **GET** /api/v2/LearningService/CourseWikis/Count | Get course wikis count
[**update_course_wiki_async**](CourseWikisApi.md#update_course_wiki_async) | **PUT** /api/v2/LearningService/CourseWikis/{wikiId} | Update a course wiki



## create_course_wiki_async

> create_course_wiki_async(tenant_id, api_version, x_api_version, course_wiki_create_dto)
Create a new course wiki

Creates a new course wiki for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_wiki_create_dto** | Option<[**CourseWikiCreateDto**](CourseWikiCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_wiki_async

> delete_course_wiki_async(tenant_id, wiki_id, api_version, x_api_version)
Delete a course wiki

Deletes a course wiki for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**wiki_id** | **String** |  | [required] |
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


## get_course_wiki_by_id_async

> models::CourseWikiDto get_course_wiki_by_id_async(wiki_id, api_version, x_api_version)
Get course wiki by ID

Retrieves a specific course wiki by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wiki_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseWikiDto**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_wikis_async

> Vec<models::CourseWikiDto> get_course_wikis_async(tenant_id, api_version, x_api_version)
Get all course wikis

Retrieves all course wikis for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseWikiDto>**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_wikis_count_async

> i32 get_course_wikis_count_async(tenant_id, api_version, x_api_version)
Get course wikis count

Returns the count of course wikis for the specified tenant.

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


## update_course_wiki_async

> update_course_wiki_async(tenant_id, wiki_id, api_version, x_api_version, course_wiki_update_dto)
Update a course wiki

Updates an existing course wiki for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**wiki_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_wiki_update_dto** | Option<[**CourseWikiUpdateDto**](CourseWikiUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

