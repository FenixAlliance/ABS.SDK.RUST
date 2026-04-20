# \SocialFeedsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_feed_post_async**](SocialFeedsApi.md#create_feed_post_async) | **POST** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts | Create a social feed post
[**delete_feed_post_async**](SocialFeedsApi.md#delete_feed_post_async) | **DELETE** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Delete a social feed post
[**get_feed_notifications**](SocialFeedsApi.md#get_feed_notifications) | **GET** /api/v2/SocialService/SocialFeeds | Get social feeds
[**get_feed_post_async**](SocialFeedsApi.md#get_feed_post_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Get social feed post by ID
[**get_feed_posts_async**](SocialFeedsApi.md#get_feed_posts_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts | Get social feed posts
[**get_feed_posts_count_async**](SocialFeedsApi.md#get_feed_posts_count_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/Count | Count social feed posts
[**get_notification_async**](SocialFeedsApi.md#get_notification_async) | **GET** /api/v2/SocialService/SocialFeeds/{socialFeedId} | Get social feed by ID
[**get_notifications_count_async**](SocialFeedsApi.md#get_notifications_count_async) | **GET** /api/v2/SocialService/SocialFeeds/Count | Count social feeds
[**update_feed_post_async**](SocialFeedsApi.md#update_feed_post_async) | **PUT** /api/v2/SocialService/SocialFeeds/{socialFeedId}/Posts/{feedPostId} | Update a social feed post



## create_feed_post_async

> models::SocialFeedPostDtoEnvelope create_feed_post_async(social_profile_id, social_feed_id, api_version, x_api_version, social_feed_post_create_dto)
Create a social feed post

Creates a new post in a specific social feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_feed_post_create_dto** | Option<[**SocialFeedPostCreateDto**](SocialFeedPostCreateDto.md)> |  |  |

### Return type

[**models::SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_feed_post_async

> models::EmptyEnvelope delete_feed_post_async(social_profile_id, social_feed_id, feed_post_id, api_version, x_api_version)
Delete a social feed post

Deletes a post from a specific social feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**feed_post_id** | **uuid::Uuid** |  | [required] |
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


## get_feed_notifications

> models::SocialFeedDtoListEnvelope get_feed_notifications(social_profile_id, api_version, x_api_version)
Get social feeds

Retrieves a list of social feeds for the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialFeedDtoListEnvelope**](SocialFeedDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_feed_post_async

> models::SocialFeedPostDtoEnvelope get_feed_post_async(social_profile_id, social_feed_id, feed_post_id, api_version, x_api_version)
Get social feed post by ID

Retrieves a specific post from a social feed by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**feed_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_feed_posts_async

> models::SocialFeedPostDtoListEnvelope get_feed_posts_async(social_profile_id, social_feed_id, api_version, x_api_version)
Get social feed posts

Retrieves a list of posts for a specific social feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialFeedPostDtoListEnvelope**](SocialFeedPostDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_feed_posts_count_async

> models::Int32Envelope get_feed_posts_count_async(social_profile_id, social_feed_id, api_version, x_api_version)
Count social feed posts

Returns the count of posts for a specific social feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
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


## get_notification_async

> models::SocialFeedDtoEnvelope get_notification_async(social_profile_id, social_feed_id, api_version, x_api_version)
Get social feed by ID

Retrieves a specific social feed by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialFeedDtoEnvelope**](SocialFeedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_notifications_count_async

> models::Int32Envelope get_notifications_count_async(social_profile_id, api_version, x_api_version)
Count social feeds

Returns the count of social feeds for the specified social profile.

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


## update_feed_post_async

> models::SocialFeedPostDtoEnvelope update_feed_post_async(social_profile_id, social_feed_id, feed_post_id, api_version, x_api_version, social_feed_post_update_dto)
Update a social feed post

Updates an existing post in a specific social feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**social_feed_id** | **uuid::Uuid** |  | [required] |
**feed_post_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_feed_post_update_dto** | Option<[**SocialFeedPostUpdateDto**](SocialFeedPostUpdateDto.md)> |  |  |

### Return type

[**models::SocialFeedPostDtoEnvelope**](SocialFeedPostDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

