# \SocialPostsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_social_post_async**](SocialPostsApi.md#create_social_post_async) | **POST** /api/v2/SocialService/SocialPosts | Create a social post
[**create_social_post_attachment_async**](SocialPostsApi.md#create_social_post_attachment_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments | Create a social post attachment
[**create_social_post_comment_async**](SocialPostsApi.md#create_social_post_comment_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments | Create a social post comment
[**create_social_post_reaction_async**](SocialPostsApi.md#create_social_post_reaction_async) | **POST** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions | Create a social post reaction
[**delete_social_post_async**](SocialPostsApi.md#delete_social_post_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId} | Delete a social post
[**delete_social_post_attachment_async**](SocialPostsApi.md#delete_social_post_attachment_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Delete a social post attachment
[**delete_social_post_comment_async**](SocialPostsApi.md#delete_social_post_comment_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Delete a social post comment
[**delete_social_post_reaction_async**](SocialPostsApi.md#delete_social_post_reaction_async) | **DELETE** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Delete a social post reaction
[**get_social_post_async**](SocialPostsApi.md#get_social_post_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId} | Get social post by ID
[**get_social_post_attachment_async**](SocialPostsApi.md#get_social_post_attachment_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Get social post attachment by ID
[**get_social_post_attachments_async**](SocialPostsApi.md#get_social_post_attachments_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments | Get social post attachments
[**get_social_post_attachments_count_async**](SocialPostsApi.md#get_social_post_attachments_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/Count | Count social post attachments
[**get_social_post_comment_async**](SocialPostsApi.md#get_social_post_comment_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Get social post comment by ID
[**get_social_post_comments_async**](SocialPostsApi.md#get_social_post_comments_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments | Get social post comments
[**get_social_post_comments_count_async**](SocialPostsApi.md#get_social_post_comments_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/Count | Count social post comments
[**get_social_post_reaction_async**](SocialPostsApi.md#get_social_post_reaction_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Get social post reaction by ID
[**get_social_post_reactions_async**](SocialPostsApi.md#get_social_post_reactions_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions | Get social post reactions
[**get_social_post_reactions_count_async**](SocialPostsApi.md#get_social_post_reactions_count_async) | **GET** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/Count | Count social post reactions
[**get_social_posts_async**](SocialPostsApi.md#get_social_posts_async) | **GET** /api/v2/SocialService/SocialPosts | Get social posts
[**get_social_posts_count_async**](SocialPostsApi.md#get_social_posts_count_async) | **GET** /api/v2/SocialService/SocialPosts/Count | Count social posts
[**update_social_post_async**](SocialPostsApi.md#update_social_post_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId} | Update a social post
[**update_social_post_attachment_async**](SocialPostsApi.md#update_social_post_attachment_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Attachments/{attachmentId} | Update a social post attachment
[**update_social_post_comment_async**](SocialPostsApi.md#update_social_post_comment_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Comments/{commentId} | Update a social post comment
[**update_social_post_reaction_async**](SocialPostsApi.md#update_social_post_reaction_async) | **PUT** /api/v2/SocialService/SocialPosts/{socialPostId}/Reactions/{reactionId} | Update a social post reaction



## create_social_post_async

> models::SocialPostDtoEnvelope create_social_post_async(social_profile_id, api_version, x_api_version, social_post_create_dto)
Create a social post

Creates a new social post for the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_create_dto** | Option<[**SocialPostCreateDto**](SocialPostCreateDto.md)> |  |  |

### Return type

[**models::SocialPostDtoEnvelope**](SocialPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_social_post_attachment_async

> models::SocialPostAttachmentDtoEnvelope create_social_post_attachment_async(social_post_id, social_profile_id, api_version, x_api_version, social_post_attachment_create_dto)
Create a social post attachment

Creates a new attachment for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_attachment_create_dto** | Option<[**SocialPostAttachmentCreateDto**](SocialPostAttachmentCreateDto.md)> |  |  |

### Return type

[**models::SocialPostAttachmentDtoEnvelope**](SocialPostAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_social_post_comment_async

> models::EmptyEnvelope create_social_post_comment_async(social_profile_id, social_post_id, api_version, x_api_version, social_post_comment_create_dto)
Create a social post comment

Creates a new comment on a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_comment_create_dto** | Option<[**SocialPostCommentCreateDto**](SocialPostCommentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_social_post_reaction_async

> models::SocialReactionDtoEnvelope create_social_post_reaction_async(social_post_id, social_profile_id, api_version, x_api_version, social_reaction_create_dto)
Create a social post reaction

Creates a new reaction on a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_reaction_create_dto** | Option<[**SocialReactionCreateDto**](SocialReactionCreateDto.md)> |  |  |

### Return type

[**models::SocialReactionDtoEnvelope**](SocialReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_social_post_async

> models::EmptyEnvelope delete_social_post_async(social_profile_id, social_post_id, api_version, x_api_version)
Delete a social post

Deletes a social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
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


## delete_social_post_attachment_async

> models::EmptyEnvelope delete_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, api_version, x_api_version)
Delete a social post attachment

Deletes an attachment from a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**attachment_id** | **uuid::Uuid** |  | [required] |
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


## delete_social_post_comment_async

> models::EmptyEnvelope delete_social_post_comment_async(social_profile_id, social_post_id, comment_id, api_version, x_api_version)
Delete a social post comment

Deletes a comment from a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**comment_id** | **uuid::Uuid** |  | [required] |
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


## delete_social_post_reaction_async

> models::EmptyEnvelope delete_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, api_version, x_api_version)
Delete a social post reaction

Deletes a reaction from a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**reaction_id** | **uuid::Uuid** |  | [required] |
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


## get_social_post_async

> models::SocialPostDtoEnvelope get_social_post_async(social_profile_id, social_post_id, api_version, x_api_version)
Get social post by ID

Retrieves a specific social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostDtoEnvelope**](SocialPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_attachment_async

> models::EmptyEnvelope get_social_post_attachment_async(social_post_id, attachment_id, api_version, x_api_version)
Get social post attachment by ID

Retrieves a specific attachment from a social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**attachment_id** | **uuid::Uuid** |  | [required] |
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


## get_social_post_attachments_async

> models::SocialPostAttachmentDtoListEnvelope get_social_post_attachments_async(social_post_id, api_version, x_api_version)
Get social post attachments

Retrieves a list of attachments for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostAttachmentDtoListEnvelope**](SocialPostAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_attachments_count_async

> models::Int32Envelope get_social_post_attachments_count_async(social_post_id, api_version, x_api_version)
Count social post attachments

Returns the count of attachments for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
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


## get_social_post_comment_async

> models::SocialPostCommentDtoEnvelope get_social_post_comment_async(social_profile_id, social_post_id, comment_id, api_version, x_api_version)
Get social post comment by ID

Retrieves a specific comment from a social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**comment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostCommentDtoEnvelope**](SocialPostCommentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_comments_async

> models::SocialPostCommentDtoListEnvelope get_social_post_comments_async(social_profile_id, social_post_id, api_version, x_api_version)
Get social post comments

Retrieves a list of comments for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostCommentDtoListEnvelope**](SocialPostCommentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_comments_count_async

> models::Int32Envelope get_social_post_comments_count_async(social_profile_id, social_post_id, api_version, x_api_version)
Count social post comments

Returns the count of comments for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
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


## get_social_post_reaction_async

> models::SocialReactionDtoEnvelope get_social_post_reaction_async(social_post_id, reaction_id, api_version, x_api_version)
Get social post reaction by ID

Retrieves a specific reaction from a social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**reaction_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialReactionDtoEnvelope**](SocialReactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_reactions_async

> models::SocialReactionDtoListEnvelope get_social_post_reactions_async(social_post_id, social_profile_id, api_version, x_api_version)
Get social post reactions

Retrieves a list of reactions for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialReactionDtoListEnvelope**](SocialReactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_reactions_count_async

> models::Int32Envelope get_social_post_reactions_count_async(social_post_id, social_profile_id, api_version, x_api_version)
Count social post reactions

Returns the count of reactions for a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_post_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
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


## get_social_posts_async

> models::SocialPostDtoListEnvelope get_social_posts_async(social_profile_id, api_version, x_api_version)
Get social posts

Retrieves a list of social posts for the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostDtoListEnvelope**](SocialPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_posts_count_async

> models::Int32Envelope get_social_posts_count_async(social_profile_id, api_version, x_api_version)
Count social posts

Returns the count of social posts for the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
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


## update_social_post_async

> models::EmptyEnvelope update_social_post_async(social_profile_id, social_post_id, api_version, x_api_version, social_post_update_dto)
Update a social post

Updates an existing social post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_update_dto** | Option<[**SocialPostUpdateDto**](SocialPostUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_post_attachment_async

> models::EmptyEnvelope update_social_post_attachment_async(social_profile_id, social_post_id, attachment_id, api_version, x_api_version, social_post_attachment_update_dto)
Update a social post attachment

Updates an existing attachment on a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_attachment_update_dto** | Option<[**SocialPostAttachmentUpdateDto**](SocialPostAttachmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_post_comment_async

> models::EmptyEnvelope update_social_post_comment_async(social_profile_id, social_post_id, comment_id, api_version, x_api_version, social_post_comment_update_dto)
Update a social post comment

Updates an existing comment on a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**comment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_post_comment_update_dto** | Option<[**SocialPostCommentUpdateDto**](SocialPostCommentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_post_reaction_async

> models::EmptyEnvelope update_social_post_reaction_async(social_profile_id, social_post_id, reaction_id, api_version, x_api_version, social_reaction_update_dto)
Update a social post reaction

Updates an existing reaction on a specific social post.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_post_id** | **uuid::Uuid** |  | [required] |
**reaction_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_reaction_update_dto** | Option<[**SocialReactionUpdateDto**](SocialReactionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

