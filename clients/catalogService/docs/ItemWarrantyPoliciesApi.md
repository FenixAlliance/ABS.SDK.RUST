# \ItemWarrantyPoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_item_warranty_policies_async**](ItemWarrantyPoliciesApi.md#count_item_warranty_policies_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies/Count | Count item warranty policies
[**get_item_warranty_policies_async**](ItemWarrantyPoliciesApi.md#get_item_warranty_policies_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies | Get item warranty policies
[**get_item_warranty_policy_by_id_async**](ItemWarrantyPoliciesApi.md#get_item_warranty_policy_by_id_async) | **GET** /api/v2/CatalogService/ItemWarrantyPolicies/{itemWarrantyPolicyId} | Get item warranty policy by ID
[**relate_item_to_warranty_policy_async**](ItemWarrantyPoliciesApi.md#relate_item_to_warranty_policy_async) | **POST** /api/v2/CatalogService/ItemWarrantyPolicies | Relate item to warranty policy
[**remove_warranty_policy_from_item_async**](ItemWarrantyPoliciesApi.md#remove_warranty_policy_from_item_async) | **DELETE** /api/v2/CatalogService/ItemWarrantyPolicies/{itemWarrantyPolicyId} | Remove warranty policy from item



## count_item_warranty_policies_async

> models::Int32Envelope count_item_warranty_policies_async(item_id, api_version, x_api_version)
Count item warranty policies

Counts all warranty policies for a specific item.

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


## get_item_warranty_policies_async

> models::ItemWarrantyPolicyDtoListEnvelope get_item_warranty_policies_async(item_id, api_version, x_api_version)
Get item warranty policies

Retrieves all warranty policies for a specific item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoListEnvelope**](ItemWarrantyPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_warranty_policy_by_id_async

> models::ItemWarrantyPolicyDtoEnvelope get_item_warranty_policy_by_id_async(item_warranty_policy_id, item_id, api_version, x_api_version)
Get item warranty policy by ID

Retrieves a specific warranty policy for an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_warranty_policy_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_item_to_warranty_policy_async

> relate_item_to_warranty_policy_async(tenant_id, item_id, warranty_policy_id, api_version, x_api_version)
Relate item to warranty policy

Relates an item to an existing warranty policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**warranty_policy_id** | **uuid::Uuid** |  | [required] |
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


## remove_warranty_policy_from_item_async

> remove_warranty_policy_from_item_async(tenant_id, item_id, item_warranty_policy_id, api_version, x_api_version)
Remove warranty policy from item

Removes a warranty policy from an item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_warranty_policy_id** | **uuid::Uuid** |  | [required] |
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

