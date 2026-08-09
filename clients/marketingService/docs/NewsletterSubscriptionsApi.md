# \NewsletterSubscriptionsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#create_newsletter_subscription_async) | **POST** /api/v2/MarketingService/NewsletterSubscriptions | Create a newsletter subscription
[**delete_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#delete_newsletter_subscription_async) | **DELETE** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Delete a newsletter subscription
[**get_newsletter_subscription_by_id_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscription_by_id_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Get newsletter subscription by ID
[**get_newsletter_subscriptions_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscriptions_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions | Get newsletter subscriptions
[**get_newsletter_subscriptions_count_async**](NewsletterSubscriptionsApi.md#get_newsletter_subscriptions_count_async) | **GET** /api/v2/MarketingService/NewsletterSubscriptions/Count | Get newsletter subscriptions count
[**update_newsletter_subscription_async**](NewsletterSubscriptionsApi.md#update_newsletter_subscription_async) | **PUT** /api/v2/MarketingService/NewsletterSubscriptions/{newsletterSubscriptionId} | Update a newsletter subscription



## create_newsletter_subscription_async

> models::EmptyEnvelope create_newsletter_subscription_async(tenant_id, newsletter_subscription_create_dto, api_version, x_api_version)
Create a newsletter subscription

Creates a new newsletter subscription for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_subscription_create_dto** | [**NewsletterSubscriptionCreateDto**](NewsletterSubscriptionCreateDto.md) |  | [required] |
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


## delete_newsletter_subscription_async

> models::EmptyEnvelope delete_newsletter_subscription_async(tenant_id, newsletter_subscription_id, api_version, x_api_version)
Delete a newsletter subscription

Deletes a newsletter subscription by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_subscription_id** | **uuid::Uuid** |  | [required] |
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


## get_newsletter_subscription_by_id_async

> models::NewsletterSubscriptionDtoEnvelope get_newsletter_subscription_by_id_async(tenant_id, newsletter_subscription_id, api_version, x_api_version)
Get newsletter subscription by ID

Retrieves the details of a specific newsletter subscription by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_subscription_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NewsletterSubscriptionDtoEnvelope**](NewsletterSubscriptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_newsletter_subscriptions_async

> models::NewsletterSubscriptionDtoListEnvelope get_newsletter_subscriptions_async(tenant_id, api_version, x_api_version, newsletter_subscription_dto_collection_query_parameters)
Get newsletter subscriptions

Retrieves a collection of newsletter subscriptions for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**newsletter_subscription_dto_collection_query_parameters** | Option<[**NewsletterSubscriptionDtoCollectionQueryParameters**](NewsletterSubscriptionDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::NewsletterSubscriptionDtoListEnvelope**](NewsletterSubscriptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_newsletter_subscriptions_count_async

> models::Int32Envelope get_newsletter_subscriptions_count_async(tenant_id, api_version, x_api_version, newsletter_subscription_dto_collection_query_parameters)
Get newsletter subscriptions count

Returns the count of newsletter subscriptions for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**newsletter_subscription_dto_collection_query_parameters** | Option<[**NewsletterSubscriptionDtoCollectionQueryParameters**](NewsletterSubscriptionDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_newsletter_subscription_async

> models::EmptyEnvelope update_newsletter_subscription_async(tenant_id, newsletter_subscription_id, newsletter_subscription_update_dto, api_version, x_api_version)
Update a newsletter subscription

Updates an existing newsletter subscription by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_subscription_id** | **uuid::Uuid** |  | [required] |
**newsletter_subscription_update_dto** | [**NewsletterSubscriptionUpdateDto**](NewsletterSubscriptionUpdateDto.md) |  | [required] |
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

