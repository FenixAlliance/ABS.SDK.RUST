# \SubscriptionPlansApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_subscription_plan_async**](SubscriptionPlansApi.md#create_subscription_plan_async) | **POST** /api/v2/SubscriptionsService/SubscriptionPlans | Create a subscription plan
[**delete_subscription_plan_async**](SubscriptionPlansApi.md#delete_subscription_plan_async) | **DELETE** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Delete a subscription plan
[**get_subscription_plan_by_id_async**](SubscriptionPlansApi.md#get_subscription_plan_by_id_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Get a subscription plan by ID
[**get_subscription_plans_async**](SubscriptionPlansApi.md#get_subscription_plans_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans | Get all subscription plans
[**get_subscription_plans_count_async**](SubscriptionPlansApi.md#get_subscription_plans_count_async) | **GET** /api/v2/SubscriptionsService/SubscriptionPlans/Count | Get subscription plans count
[**update_subscription_plan_async**](SubscriptionPlansApi.md#update_subscription_plan_async) | **PUT** /api/v2/SubscriptionsService/SubscriptionPlans/{planId} | Update a subscription plan



## create_subscription_plan_async

> models::Envelope create_subscription_plan_async(tenant_id, api_version, x_api_version, subscription_plan_create_dto)
Create a subscription plan

Creates a new subscription plan for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**subscription_plan_create_dto** | Option<[**SubscriptionPlanCreateDto**](SubscriptionPlanCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_subscription_plan_async

> models::Envelope delete_subscription_plan_async(tenant_id, plan_id, api_version, x_api_version)
Delete a subscription plan

Deletes a subscription plan by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**plan_id** | **uuid::Uuid** |  | [required] |
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


## get_subscription_plan_by_id_async

> models::SubscriptionPlanDtoEnvelope get_subscription_plan_by_id_async(tenant_id, plan_id, api_version, x_api_version)
Get a subscription plan by ID

Retrieves a subscription plan by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**plan_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SubscriptionPlanDtoEnvelope**](SubscriptionPlanDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscription_plans_async

> models::SubscriptionPlanDtoIReadOnlyListEnvelope get_subscription_plans_async(tenant_id, api_version, x_api_version)
Get all subscription plans

Retrieves all subscription plans for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SubscriptionPlanDtoIReadOnlyListEnvelope**](SubscriptionPlanDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscription_plans_count_async

> models::Int32Envelope get_subscription_plans_count_async(tenant_id, api_version, x_api_version)
Get subscription plans count

Returns the count of subscription plans for the specified tenant.

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


## update_subscription_plan_async

> models::Envelope update_subscription_plan_async(tenant_id, plan_id, api_version, x_api_version, subscription_plan_update_dto)
Update a subscription plan

Updates an existing subscription plan.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**plan_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**subscription_plan_update_dto** | Option<[**SubscriptionPlanUpdateDto**](SubscriptionPlanUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

