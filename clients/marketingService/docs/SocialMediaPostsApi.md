# \SocialMediaPostsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_social_media_post_async**](SocialMediaPostsApi.md#create_social_media_post_async) | **POST** /api/v2/MarketingService/SocialMediaPosts | Create a social media post
[**delete_social_media_post_async**](SocialMediaPostsApi.md#delete_social_media_post_async) | **DELETE** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Delete a social media post
[**get_social_media_post_details_async**](SocialMediaPostsApi.md#get_social_media_post_details_async) | **GET** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Get social media post by ID
[**get_social_media_posts_count_async**](SocialMediaPostsApi.md#get_social_media_posts_count_async) | **GET** /api/v2/MarketingService/SocialMediaPosts/Count | Get social media posts count
[**get_social_media_posts_o_data_async**](SocialMediaPostsApi.md#get_social_media_posts_o_data_async) | **GET** /api/v2/MarketingService/SocialMediaPosts | Get social media posts
[**update_social_media_post_async**](SocialMediaPostsApi.md#update_social_media_post_async) | **PUT** /api/v2/MarketingService/SocialMediaPosts/{socialmediapostId} | Update a social media post



## create_social_media_post_async

> models::EmptyEnvelope create_social_media_post_async(tenant_id, social_media_post_create_dto, api_version, x_api_version)
Create a social media post

Creates a new social media post for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**social_media_post_create_dto** | [**SocialMediaPostCreateDto**](SocialMediaPostCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_social_media_post_async

> models::EmptyEnvelope delete_social_media_post_async(tenant_id, socialmediapost_id, api_version, x_api_version)
Delete a social media post

Deletes a social media post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialmediapost_id** | **uuid::Uuid** |  | [required] |
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


## get_social_media_post_details_async

> models::SocialMediaPostDtoEnvelope get_social_media_post_details_async(tenant_id, socialmediapost_id, api_version, x_api_version)
Get social media post by ID

Retrieves the details of a specific social media post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialmediapost_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialMediaPostDtoEnvelope**](SocialMediaPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_media_posts_count_async

> models::Int32Envelope get_social_media_posts_count_async(tenant_id, api_version, x_api_version)
Get social media posts count

Returns the count of social media posts for the specified tenant using OData query options.

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


## get_social_media_posts_o_data_async

> models::SocialMediaPostDtoListEnvelope get_social_media_posts_o_data_async(tenant_id, api_version, x_api_version)
Get social media posts

Retrieves a collection of social media posts for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialMediaPostDtoListEnvelope**](SocialMediaPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_media_post_async

> models::EmptyEnvelope update_social_media_post_async(tenant_id, socialmediapost_id, social_media_post_update_dto, api_version, x_api_version)
Update a social media post

Updates an existing social media post by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialmediapost_id** | **uuid::Uuid** |  | [required] |
**social_media_post_update_dto** | [**SocialMediaPostUpdateDto**](SocialMediaPostUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

