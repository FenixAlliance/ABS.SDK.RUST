# \BlogPostAuthorsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_blog_posts_by_author_async**](BlogPostAuthorsApi.md#count_blog_posts_by_author_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId}/BlogPosts/Count | Count blog posts by author
[**get_blog_author_by_id_async**](BlogPostAuthorsApi.md#get_blog_author_by_id_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId} | Get blog author by ID
[**get_blog_authors_async**](BlogPostAuthorsApi.md#get_blog_authors_async) | **GET** /api/v2/ContentService/BlogPostAuthors | Get blog authors
[**get_blog_posts_by_author_async**](BlogPostAuthorsApi.md#get_blog_posts_by_author_async) | **GET** /api/v2/ContentService/BlogPostAuthors/{authorId}/BlogPosts | Get blog posts by author



## count_blog_posts_by_author_async

> models::Int32Envelope count_blog_posts_by_author_async(author_id, api_version, x_api_version)
Count blog posts by author

Returns the count of blog posts written by a specific author.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**author_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_author_by_id_async

> models::BlogAuthorDtoEnvelope get_blog_author_by_id_async(author_id, api_version, x_api_version)
Get blog author by ID

Retrieves a specific blog author by their identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**author_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogAuthorDtoEnvelope**](BlogAuthorDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_authors_async

> models::BlogAuthorDtoListEnvelope get_blog_authors_async(tenant_id, api_version, x_api_version)
Get blog authors

Retrieves all blog authors, optionally filtered by tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogAuthorDtoListEnvelope**](BlogAuthorDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_posts_by_author_async

> models::BlogPostDtoListEnvelope get_blog_posts_by_author_async(author_id, api_version, x_api_version)
Get blog posts by author

Retrieves all blog posts written by a specific author.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**author_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogPostDtoListEnvelope**](BlogPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

