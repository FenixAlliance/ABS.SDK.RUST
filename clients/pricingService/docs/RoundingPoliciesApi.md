# \RoundingPoliciesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_rounding_policy_async**](RoundingPoliciesApi.md#create_rounding_policy_async) | **POST** /api/v2/PricingService/RoundingPolicies | Creates a rounding policy
[**delete_rounding_policy_async**](RoundingPoliciesApi.md#delete_rounding_policy_async) | **DELETE** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Deletes a rounding policy
[**get_rounding_policies_async**](RoundingPoliciesApi.md#get_rounding_policies_async) | **GET** /api/v2/PricingService/RoundingPolicies | Gets all rounding policies
[**get_rounding_policies_count_async**](RoundingPoliciesApi.md#get_rounding_policies_count_async) | **GET** /api/v2/PricingService/RoundingPolicies/Count | Counts rounding policies
[**get_rounding_policy_by_id_async**](RoundingPoliciesApi.md#get_rounding_policy_by_id_async) | **GET** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Gets a rounding policy by ID
[**update_rounding_policy_async**](RoundingPoliciesApi.md#update_rounding_policy_async) | **PUT** /api/v2/PricingService/RoundingPolicies/{roundingPolicyId} | Updates a rounding policy



## create_rounding_policy_async

> models::EmptyEnvelope create_rounding_policy_async(tenant_id, rounding_policy_create_dto, api_version, x_api_version)
Creates a rounding policy

Creates a new rounding policy for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rounding_policy_create_dto** | [**RoundingPolicyCreateDto**](RoundingPolicyCreateDto.md) |  | [required] |
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


## delete_rounding_policy_async

> models::EmptyEnvelope delete_rounding_policy_async(tenant_id, rounding_policy_id, api_version, x_api_version)
Deletes a rounding policy

Deletes the specified rounding policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rounding_policy_id** | **uuid::Uuid** |  | [required] |
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


## get_rounding_policies_async

> models::RoundingPolicyDtoListEnvelope get_rounding_policies_async(tenant_id, api_version, x_api_version)
Gets all rounding policies

Retrieves all rounding policies for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RoundingPolicyDtoListEnvelope**](RoundingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_rounding_policies_count_async

> models::Int32Envelope get_rounding_policies_count_async(tenant_id, api_version, x_api_version)
Counts rounding policies

Gets the count of rounding policies for the current tenant.

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


## get_rounding_policy_by_id_async

> models::RoundingPolicyDtoEnvelope get_rounding_policy_by_id_async(tenant_id, rounding_policy_id, api_version, x_api_version)
Gets a rounding policy by ID

Retrieves the details of a rounding policy using its unique ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rounding_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RoundingPolicyDtoEnvelope**](RoundingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_rounding_policy_async

> models::EmptyEnvelope update_rounding_policy_async(tenant_id, rounding_policy_id, rounding_policy_update_dto, api_version, x_api_version)
Updates a rounding policy

Updates the specified rounding policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**rounding_policy_id** | **uuid::Uuid** |  | [required] |
**rounding_policy_update_dto** | [**RoundingPolicyUpdateDto**](RoundingPolicyUpdateDto.md) |  | [required] |
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

