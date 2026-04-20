# \ItemRefundPoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_refund_policies_async**](ItemRefundPoliciesApi.md#count_item_refund_policies_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies/Count | Count item refund policies
[**get_item_refund_policies_async**](ItemRefundPoliciesApi.md#get_item_refund_policies_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies | Get item refund policies
[**get_item_refund_policy_by_id_async**](ItemRefundPoliciesApi.md#get_item_refund_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemRefundPolicies/{itemRefundPolicyId} | Get item refund policy by ID
[**relate_item_to_refund_policy_async**](ItemRefundPoliciesApi.md#relate_item_to_refund_policy_async) | **POST** /api/v2/CatalogService/ItemRefundPolicies | Relate item to refund policy
[**remove_refund_policy_from_item_async**](ItemRefundPoliciesApi.md#remove_refund_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemRefundPolicies/{itemRefundPolicyId} | Remove refund policy from item



## count_item_refund_policies_async

> models::Int32Envelope count_item_refund_policies_async(item_id, api_version, x_api_version)
Count item refund policies

Counts all refund policies for a specific item.

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


## get_item_refund_policies_async

> models::ItemRefundPolicyDtoListEnvelope get_item_refund_policies_async(item_id, api_version, x_api_version)
Get item refund policies

Retrieves all refund policies for a specific item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoListEnvelope**](ItemRefundPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_refund_policy_by_id_async

> models::ItemRefundPolicyDtoEnvelope get_item_refund_policy_by_id_async(item_refund_policy_id, item_id, api_version, x_api_version)
Get item refund policy by ID

Retrieves a specific refund policy for an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_refund_policy_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_item_to_refund_policy_async

> relate_item_to_refund_policy_async(tenant_id, item_id, refund_policy_id, api_version, x_api_version)
Relate item to refund policy

Relates an item to an existing refund policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**refund_policy_id** | **uuid::Uuid** |  | [required] |
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


## remove_refund_policy_from_item_async

> remove_refund_policy_from_item_async(tenant_id, item_id, item_refund_policy_id, api_version, x_api_version)
Remove refund policy from item

Removes a refund policy from an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_refund_policy_id** | **uuid::Uuid** |  | [required] |
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

