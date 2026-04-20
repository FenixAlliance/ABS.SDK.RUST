# \ItemShippingPoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_shipping_policies_async**](ItemShippingPoliciesApi.md#count_item_shipping_policies_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies/Count | Count item shipping policies
[**get_item_shipping_policies_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies | Get item shipping policies
[**get_item_shipping_policy_by_id_async**](ItemShippingPoliciesApi.md#get_item_shipping_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemShippingPolicies/{itemShippingPolicyId} | Get item shipping policy by ID
[**relate_item_to_shipping_policy_async**](ItemShippingPoliciesApi.md#relate_item_to_shipping_policy_async) | **POST** /api/v2/CatalogService/ItemShippingPolicies | Relate item to shipping policy
[**remove_shipping_policy_from_item_async**](ItemShippingPoliciesApi.md#remove_shipping_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemShippingPolicies/{itemShippingPolicyId} | Remove shipping policy from item



## count_item_shipping_policies_async

> models::Int32Envelope count_item_shipping_policies_async(item_id, api_version, x_api_version)
Count item shipping policies

Counts all shipping policies for a specific item.

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


## get_item_shipping_policies_async

> models::ItemShippingPolicyDtoListEnvelope get_item_shipping_policies_async(item_id, api_version, x_api_version)
Get item shipping policies

Retrieves all shipping policies for a specific item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoListEnvelope**](ItemShippingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_shipping_policy_by_id_async

> models::ItemShippingPolicyDtoEnvelope get_item_shipping_policy_by_id_async(item_shipping_policy_id, item_id, api_version, x_api_version)
Get item shipping policy by ID

Retrieves a specific shipping policy for an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_shipping_policy_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_item_to_shipping_policy_async

> relate_item_to_shipping_policy_async(tenant_id, item_id, shipping_policy_id, api_version, x_api_version)
Relate item to shipping policy

Relates an item to an existing shipping policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**shipping_policy_id** | **uuid::Uuid** |  | [required] |
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


## remove_shipping_policy_from_item_async

> remove_shipping_policy_from_item_async(tenant_id, item_id, item_shipping_policy_id, api_version, x_api_version)
Remove shipping policy from item

Removes a shipping policy from an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_shipping_policy_id** | **uuid::Uuid** |  | [required] |
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

