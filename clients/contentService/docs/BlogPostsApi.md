# \BlogPostsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_blog_post_async**](BlogPostsApi.md#create_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts | Create a new blog post
[**create_category_for_blog_post_async**](BlogPostsApi.md#create_category_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories | Create a category for a blog post
[**create_comment_for_blog_post_async**](BlogPostsApi.md#create_comment_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments | Create a comment for a blog post
[**create_tag_for_blog_post_async**](BlogPostsApi.md#create_tag_for_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags | Create a tag for a blog post
[**delete_blog_post_async**](BlogPostsApi.md#delete_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId} | Delete a blog post
[**delete_comment_from_blog_post_async**](BlogPostsApi.md#delete_comment_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId} | Delete a blog post comment
[**get_blog_post_by_id_async**](BlogPostsApi.md#get_blog_post_by_id_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId} | Get a blog post by ID
[**get_blog_posts_async**](BlogPostsApi.md#get_blog_posts_async) | **GET** /api/v2/ContentService/BlogPosts | Retrieve a list of blog posts
[**get_blog_posts_count_async**](BlogPostsApi.md#get_blog_posts_count_async) | **GET** /api/v2/ContentService/BlogPosts/Count | Get the count of blog posts
[**get_categories_for_blog_post_async**](BlogPostsApi.md#get_categories_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories | Get categories for a blog post
[**get_comments_for_blog_post_async**](BlogPostsApi.md#get_comments_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments | Get comments for a blog post
[**get_replies_for_comment_async**](BlogPostsApi.md#get_replies_for_comment_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId}/Replies | Get replies for a comment
[**get_tags_for_blog_post_async**](BlogPostsApi.md#get_tags_for_blog_post_async) | **GET** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags | Get tags for a blog post
[**relate_category_to_blog_post_async**](BlogPostsApi.md#relate_category_to_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories/{categoryId} | Relate an existing category to a blog post
[**relate_tag_to_blog_post_async**](BlogPostsApi.md#relate_tag_to_blog_post_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags/{tagId} | Relate an existing tag to a blog post
[**reply_to_comment_async**](BlogPostsApi.md#reply_to_comment_async) | **POST** /api/v2/ContentService/BlogPosts/{blogPostId}/Comments/{commentId}/Reply | Reply to a blog post comment
[**unrelate_category_from_blog_post_async**](BlogPostsApi.md#unrelate_category_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Categories/{categoryId} | Remove a category from a blog post
[**unrelate_tag_from_blog_post_async**](BlogPostsApi.md#unrelate_tag_from_blog_post_async) | **DELETE** /api/v2/ContentService/BlogPosts/{blogPostId}/Tags/{tagId} | Remove a tag from a blog post
[**update_blog_post_async**](BlogPostsApi.md#update_blog_post_async) | **PUT** /api/v2/ContentService/BlogPosts/{blogPostId} | Update a blog post



## create_blog_post_async

> models::EmptyEnvelope create_blog_post_async(tenant_id, blog_post_create_dto)
Create a new blog post

Creates a new blog post for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_create_dto** | Option<[**BlogPostCreateDto**](BlogPostCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_category_for_blog_post_async

> models::EmptyEnvelope create_category_for_blog_post_async(tenant_id, blog_post_id, blog_post_category_create_dto)
Create a category for a blog post

Creates a new category and relates it to a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**blog_post_category_create_dto** | Option<[**BlogPostCategoryCreateDto**](BlogPostCategoryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_comment_for_blog_post_async

> models::EmptyEnvelope create_comment_for_blog_post_async(tenant_id, blog_post_id, blog_post_comment_create_dto)
Create a comment for a blog post

Creates a new comment on a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**blog_post_comment_create_dto** | Option<[**BlogPostCommentCreateDto**](BlogPostCommentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tag_for_blog_post_async

> models::EmptyEnvelope create_tag_for_blog_post_async(tenant_id, blog_post_id, blog_post_tag_create_dto)
Create a tag for a blog post

Creates a new tag and relates it to a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**blog_post_tag_create_dto** | Option<[**BlogPostTagCreateDto**](BlogPostTagCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_blog_post_async

> models::EmptyEnvelope delete_blog_post_async(tenant_id, blog_post_id)
Delete a blog post

Deletes a blog post for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_comment_from_blog_post_async

> models::EmptyEnvelope delete_comment_from_blog_post_async(tenant_id, blog_post_id, comment_id)
Delete a blog post comment

Deletes a comment from a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**comment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_post_by_id_async

> models::BlogPostDtoEnvelope get_blog_post_by_id_async(blog_post_id)
Get a blog post by ID

Retrieves a single blog post by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**blog_post_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::BlogPostDtoEnvelope**](BlogPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_posts_async

> models::BlogPostDtoListEnvelope get_blog_posts_async(tenant_id)
Retrieve a list of blog posts

Retrieves all blog posts, optionally filtered by tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::BlogPostDtoListEnvelope**](BlogPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_posts_count_async

> models::Int32Envelope get_blog_posts_count_async(tenant_id)
Get the count of blog posts

Returns the total count of blog posts, optionally filtered by tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_categories_for_blog_post_async

> models::BlogPostCategoryDtoListEnvelope get_categories_for_blog_post_async(blog_post_id)
Get categories for a blog post

Retrieves all categories related to a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**blog_post_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::BlogPostCategoryDtoListEnvelope**](BlogPostCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_comments_for_blog_post_async

> models::BlogPostCommentDtoListEnvelope get_comments_for_blog_post_async(blog_post_id)
Get comments for a blog post

Retrieves all comments for a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**blog_post_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::BlogPostCommentDtoListEnvelope**](BlogPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_replies_for_comment_async

> models::BlogPostCommentDtoListEnvelope get_replies_for_comment_async(comment_id, blog_post_id)
Get replies for a comment

Retrieves all replies for a specific blog post comment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**comment_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **String** |  | [required] |

### Return type

[**models::BlogPostCommentDtoListEnvelope**](BlogPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tags_for_blog_post_async

> models::BlogPostTagDtoListEnvelope get_tags_for_blog_post_async(blog_post_id)
Get tags for a blog post

Retrieves all tags related to a specific blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**blog_post_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::BlogPostTagDtoListEnvelope**](BlogPostTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_category_to_blog_post_async

> models::EmptyEnvelope relate_category_to_blog_post_async(tenant_id, blog_post_id, category_id)
Relate an existing category to a blog post

Creates a relationship between an existing category and a blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_tag_to_blog_post_async

> models::EmptyEnvelope relate_tag_to_blog_post_async(tenant_id, blog_post_id, tag_id)
Relate an existing tag to a blog post

Creates a relationship between an existing tag and a blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**tag_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## reply_to_comment_async

> models::EmptyEnvelope reply_to_comment_async(tenant_id, blog_post_id, comment_id, blog_post_comment_create_dto)
Reply to a blog post comment

Creates a reply to an existing comment on a blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**comment_id** | **uuid::Uuid** |  | [required] |
**blog_post_comment_create_dto** | Option<[**BlogPostCommentCreateDto**](BlogPostCommentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## unrelate_category_from_blog_post_async

> models::EmptyEnvelope unrelate_category_from_blog_post_async(tenant_id, blog_post_id, category_id)
Remove a category from a blog post

Removes the relationship between a category and a blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## unrelate_tag_from_blog_post_async

> models::EmptyEnvelope unrelate_tag_from_blog_post_async(tenant_id, blog_post_id, tag_id)
Remove a tag from a blog post

Removes the relationship between a tag and a blog post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**tag_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_blog_post_async

> models::EmptyEnvelope update_blog_post_async(tenant_id, blog_post_id, blog_post_update_dto)
Update a blog post

Updates an existing blog post for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_id** | **uuid::Uuid** |  | [required] |
**blog_post_update_dto** | Option<[**BlogPostUpdateDto**](BlogPostUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

