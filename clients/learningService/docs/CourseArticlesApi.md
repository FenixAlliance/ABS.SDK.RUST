# \CourseArticlesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_article_async**](CourseArticlesApi.md#create_course_article_async) | **POST** /api/v2/LearningService/CourseArticles | Create a new course article
[**delete_course_article_async**](CourseArticlesApi.md#delete_course_article_async) | **DELETE** /api/v2/LearningService/CourseArticles/{articleId} | Delete a course article
[**get_course_article_by_id_async**](CourseArticlesApi.md#get_course_article_by_id_async) | **GET** /api/v2/LearningService/CourseArticles/{articleId} | Get course article by ID
[**get_course_articles_async**](CourseArticlesApi.md#get_course_articles_async) | **GET** /api/v2/LearningService/CourseArticles | Get all course articles
[**get_course_articles_count_async**](CourseArticlesApi.md#get_course_articles_count_async) | **GET** /api/v2/LearningService/CourseArticles/Count | Get course articles count
[**update_course_article_async**](CourseArticlesApi.md#update_course_article_async) | **PUT** /api/v2/LearningService/CourseArticles/{articleId} | Update a course article



## create_course_article_async

> create_course_article_async(tenant_id, api_version, x_api_version, course_article_create_dto)
Create a new course article

Creates a new course article for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_article_create_dto** | Option<[**CourseArticleCreateDto**](CourseArticleCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_article_async

> delete_course_article_async(tenant_id, article_id, api_version, x_api_version)
Delete a course article

Deletes a course article for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**article_id** | **String** |  | [required] |
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


## get_course_article_by_id_async

> models::CourseArticleDto get_course_article_by_id_async(article_id, api_version, x_api_version)
Get course article by ID

Retrieves a specific course article by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**article_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseArticleDto**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_articles_async

> Vec<models::CourseArticleDto> get_course_articles_async(tenant_id, api_version, x_api_version)
Get all course articles

Retrieves all course articles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseArticleDto>**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_articles_count_async

> i32 get_course_articles_count_async(tenant_id, api_version, x_api_version)
Get course articles count

Returns the count of course articles for the specified tenant.

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


## update_course_article_async

> update_course_article_async(tenant_id, article_id, api_version, x_api_version, course_article_update_dto)
Update a course article

Updates an existing course article for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**article_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_article_update_dto** | Option<[**CourseArticleUpdateDto**](CourseArticleUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

