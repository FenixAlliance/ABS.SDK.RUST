# \ItemShippingPoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_shipping_policy_async**](ItemShippingPoliciesApi.md#create_item_shipping_policy_async) | **POST** /api/v2/ShipmentsService/ItemShippingPolicies | Create an item shipping policy
[**delete_item_shipping_policy_async**](ItemShippingPoliciesApi.md#delete_item_shipping_policy_async) | **DELETE** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Delete an item shipping policy
[**get_item_shipping_policies_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies | Get all item shipping policies
[**get_item_shipping_policies_count_async**](ItemShippingPoliciesApi.md#get_item_shipping_policies_count_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies/Count | Get item shipping policies count
[**get_item_shipping_policy_by_id_async**](ItemShippingPoliciesApi.md#get_item_shipping_policy_by_id_async) | **GET** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Get item shipping policy by ID
[**update_item_shipping_policy_async**](ItemShippingPoliciesApi.md#update_item_shipping_policy_async) | **PUT** /api/v2/ShipmentsService/ItemShippingPolicies/{policyId} | Update an item shipping policy



## create_item_shipping_policy_async

> create_item_shipping_policy_async(tenant_id, api_version, x_api_version, item_shipping_policy_create_dto)
Create an item shipping policy

Creates a new item shipping policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_shipping_policy_create_dto** | Option<[**ItemShippingPolicyCreateDto**](ItemShippingPolicyCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_shipping_policy_async

> delete_item_shipping_policy_async(tenant_id, policy_id, api_version, x_api_version)
Delete an item shipping policy

Deletes an item shipping policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**policy_id** | **uuid::Uuid** |  | [required] |
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


## get_item_shipping_policies_async

> models::ItemShippingPolicyDtoListEnvelope get_item_shipping_policies_async(tenant_id, api_version, x_api_version)
Get all item shipping policies

Retrieves all item shipping policies for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_item_shipping_policies_count_async

> models::Int32Envelope get_item_shipping_policies_count_async(tenant_id, api_version, x_api_version)
Get item shipping policies count

Returns the count of item shipping policies.

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


## get_item_shipping_policy_by_id_async

> models::ItemShippingPolicyDtoEnvelope get_item_shipping_policy_by_id_async(tenant_id, policy_id, api_version, x_api_version)
Get item shipping policy by ID

Retrieves a specific item shipping policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**policy_id** | **uuid::Uuid** |  | [required] |
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


## update_item_shipping_policy_async

> update_item_shipping_policy_async(tenant_id, policy_id, api_version, x_api_version, item_shipping_policy_update_dto)
Update an item shipping policy

Updates an existing item shipping policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_shipping_policy_update_dto** | Option<[**ItemShippingPolicyUpdateDto**](ItemShippingPolicyUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

