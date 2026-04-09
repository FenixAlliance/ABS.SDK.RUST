# \SubscriptionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_subscription_async**](SubscriptionsApi.md#create_subscription_async) | **POST** /api/v2/SubscriptionsService/Subscriptions | Create a subscription
[**delete_subscription_async**](SubscriptionsApi.md#delete_subscription_async) | **DELETE** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Delete a subscription
[**get_subscription_by_id_async**](SubscriptionsApi.md#get_subscription_by_id_async) | **GET** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Get a subscription by ID
[**get_subscriptions_async**](SubscriptionsApi.md#get_subscriptions_async) | **GET** /api/v2/SubscriptionsService/Subscriptions | Get all subscriptions
[**get_subscriptions_count_async**](SubscriptionsApi.md#get_subscriptions_count_async) | **GET** /api/v2/SubscriptionsService/Subscriptions/Count | Get subscriptions count
[**update_subscription_async**](SubscriptionsApi.md#update_subscription_async) | **PUT** /api/v2/SubscriptionsService/Subscriptions/{subscriptionId} | Update a subscription



## create_subscription_async

> models::Envelope create_subscription_async(tenant_id, api_version, x_api_version, subscription_create_dto)
Create a subscription

Creates a new subscription for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**subscription_create_dto** | Option<[**SubscriptionCreateDto**](SubscriptionCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_subscription_async

> models::Envelope delete_subscription_async(tenant_id, subscription_id, api_version, x_api_version)
Delete a subscription

Deletes a subscription by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**subscription_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscription_by_id_async

> models::SubscriptionDtoEnvelope get_subscription_by_id_async(tenant_id, subscription_id, api_version, x_api_version)
Get a subscription by ID

Retrieves a subscription by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**subscription_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SubscriptionDtoEnvelope**](SubscriptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscriptions_async

> models::SubscriptionDtoIReadOnlyListEnvelope get_subscriptions_async(tenant_id, api_version, x_api_version)
Get all subscriptions

Retrieves all subscriptions for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SubscriptionDtoIReadOnlyListEnvelope**](SubscriptionDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscriptions_count_async

> models::Int32Envelope get_subscriptions_count_async(tenant_id, api_version, x_api_version)
Get subscriptions count

Returns the count of subscriptions for the specified tenant.

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


## update_subscription_async

> models::Envelope update_subscription_async(tenant_id, subscription_id, api_version, x_api_version, subscription_update_dto)
Update a subscription

Updates an existing subscription.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**subscription_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**subscription_update_dto** | Option<[**SubscriptionUpdateDto**](SubscriptionUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

