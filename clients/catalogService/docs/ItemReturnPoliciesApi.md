# \ItemReturnPoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_return_policies_async**](ItemReturnPoliciesApi.md#count_item_return_policies_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies/Count | Count item return policies
[**get_item_return_policies_async**](ItemReturnPoliciesApi.md#get_item_return_policies_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies | Get item return policies
[**get_item_return_policy_by_id_async**](ItemReturnPoliciesApi.md#get_item_return_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemReturnPolicies/{itemReturnPolicyId} | Get item return policy by ID
[**relate_item_to_return_policy_async**](ItemReturnPoliciesApi.md#relate_item_to_return_policy_async) | **POST** /api/v2/CatalogService/ItemReturnPolicies | Relate item to return policy
[**remove_return_policy_from_item_async**](ItemReturnPoliciesApi.md#remove_return_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemReturnPolicies/{itemReturnPolicyId} | Remove return policy from item



## count_item_return_policies_async

> models::Int32Envelope count_item_return_policies_async(item_id, api_version, x_api_version)
Count item return policies

Counts all return policies for a specific item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | Option<**uuid::Uuid**> |  |  |
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


## get_item_return_policies_async

> models::ItemReturnPolicyDtoListEnvelope get_item_return_policies_async(item_id, api_version, x_api_version)
Get item return policies

Retrieves all return policies for a specific item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoListEnvelope**](ItemReturnPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_return_policy_by_id_async

> models::ItemReturnPolicyDtoEnvelope get_item_return_policy_by_id_async(item_return_policy_id, item_id, api_version, x_api_version)
Get item return policy by ID

Retrieves a specific return policy for an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_return_policy_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_item_to_return_policy_async

> relate_item_to_return_policy_async(tenant_id, item_id, return_policy_id, api_version, x_api_version)
Relate item to return policy

Relates an item to an existing return policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_return_policy_from_item_async

> remove_return_policy_from_item_async(tenant_id, item_id, item_return_policy_id, api_version, x_api_version)
Remove return policy from item

Removes a return policy from an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

