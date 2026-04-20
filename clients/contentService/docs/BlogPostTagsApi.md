# \BlogPostTagsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_blog_post_tags_async**](BlogPostTagsApi.md#count_blog_post_tags_async) | **GET** /api/v2/ContentService/BlogPostTags/Count | Count blog post tags
[**create_blog_post_tag_async**](BlogPostTagsApi.md#create_blog_post_tag_async) | **POST** /api/v2/ContentService/BlogPostTags | Create a blog post tag
[**delete_blog_post_tag_async**](BlogPostTagsApi.md#delete_blog_post_tag_async) | **DELETE** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Delete a blog post tag
[**get_blog_post_tag_by_id_async**](BlogPostTagsApi.md#get_blog_post_tag_by_id_async) | **GET** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Get blog post tag by ID
[**get_blog_post_tags_async**](BlogPostTagsApi.md#get_blog_post_tags_async) | **GET** /api/v2/ContentService/BlogPostTags | Get blog post tags
[**update_blog_post_tag_async**](BlogPostTagsApi.md#update_blog_post_tag_async) | **PUT** /api/v2/ContentService/BlogPostTags/{blogPostTagId} | Update a blog post tag



## count_blog_post_tags_async

> models::Int32Envelope count_blog_post_tags_async(tenant_id, api_version, x_api_version)
Count blog post tags

Counts all blog post tags for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## create_blog_post_tag_async

> models::EmptyEnvelope create_blog_post_tag_async(tenant_id, api_version, x_api_version, blog_post_tag_create_dto)
Create a blog post tag

Creates a new blog post tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blog_post_tag_create_dto** | Option<[**BlogPostTagCreateDto**](BlogPostTagCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_blog_post_tag_async

> models::EmptyEnvelope delete_blog_post_tag_async(tenant_id, blog_post_tag_id, api_version, x_api_version)
Delete a blog post tag

Deletes a blog post tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_post_tag_by_id_async

> models::BlogPostTagDtoEnvelope get_blog_post_tag_by_id_async(tenant_id, blog_post_tag_id, api_version, x_api_version)
Get blog post tag by ID

Retrieves a specific blog post tag by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogPostTagDtoEnvelope**](BlogPostTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_post_tags_async

> models::BlogPostTagDtoListEnvelope get_blog_post_tags_async(tenant_id, api_version, x_api_version)
Get blog post tags

Retrieves all blog post tags for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogPostTagDtoListEnvelope**](BlogPostTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_blog_post_tag_async

> models::EmptyEnvelope update_blog_post_tag_async(tenant_id, blog_post_tag_id, api_version, x_api_version, blog_post_tag_update_dto)
Update a blog post tag

Updates an existing blog post tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blog_post_tag_update_dto** | Option<[**BlogPostTagUpdateDto**](BlogPostTagUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

