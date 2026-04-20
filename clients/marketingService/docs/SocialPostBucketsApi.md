# \SocialPostBucketsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_social_post_bucket_async**](SocialPostBucketsApi.md#create_social_post_bucket_async) | **POST** /api/v2/MarketingService/SocialPostBuckets | Create a social post bucket
[**delete_social_post_bucket_async**](SocialPostBucketsApi.md#delete_social_post_bucket_async) | **DELETE** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Delete a social post bucket
[**get_social_post_bucket_details_async**](SocialPostBucketsApi.md#get_social_post_bucket_details_async) | **GET** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Get social post bucket by ID
[**get_social_post_buckets_count_async**](SocialPostBucketsApi.md#get_social_post_buckets_count_async) | **GET** /api/v2/MarketingService/SocialPostBuckets/Count | Get social post buckets count
[**get_social_post_buckets_o_data_async**](SocialPostBucketsApi.md#get_social_post_buckets_o_data_async) | **GET** /api/v2/MarketingService/SocialPostBuckets | Get social post buckets
[**update_social_post_bucket_async**](SocialPostBucketsApi.md#update_social_post_bucket_async) | **PUT** /api/v2/MarketingService/SocialPostBuckets/{socialpostbucketId} | Update a social post bucket



## create_social_post_bucket_async

> models::EmptyEnvelope create_social_post_bucket_async(tenant_id, social_post_bucket_create_dto, api_version, x_api_version)
Create a social post bucket

Creates a new social post bucket for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**social_post_bucket_create_dto** | [**SocialPostBucketCreateDto**](SocialPostBucketCreateDto.md) |  | [required] |
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


## delete_social_post_bucket_async

> models::EmptyEnvelope delete_social_post_bucket_async(tenant_id, socialpostbucket_id, api_version, x_api_version)
Delete a social post bucket

Deletes a social post bucket by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialpostbucket_id** | **uuid::Uuid** |  | [required] |
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


## get_social_post_bucket_details_async

> models::SocialPostBucketDtoEnvelope get_social_post_bucket_details_async(tenant_id, socialpostbucket_id, api_version, x_api_version)
Get social post bucket by ID

Retrieves the details of a specific social post bucket by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialpostbucket_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostBucketDtoEnvelope**](SocialPostBucketDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_post_buckets_count_async

> models::Int32Envelope get_social_post_buckets_count_async(tenant_id, api_version, x_api_version)
Get social post buckets count

Returns the count of social post buckets for the specified tenant using OData query options.

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


## get_social_post_buckets_o_data_async

> models::SocialPostBucketDtoListEnvelope get_social_post_buckets_o_data_async(tenant_id, api_version, x_api_version)
Get social post buckets

Retrieves a collection of social post buckets for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialPostBucketDtoListEnvelope**](SocialPostBucketDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_post_bucket_async

> models::EmptyEnvelope update_social_post_bucket_async(tenant_id, socialpostbucket_id, social_post_bucket_update_dto, api_version, x_api_version)
Update a social post bucket

Updates an existing social post bucket by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**socialpostbucket_id** | **uuid::Uuid** |  | [required] |
**social_post_bucket_update_dto** | [**SocialPostBucketUpdateDto**](SocialPostBucketUpdateDto.md) |  | [required] |
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

