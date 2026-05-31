# \RefundPoliciesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_refund_policy_async**](RefundPoliciesApi.md#create_refund_policy_async) | **POST** /api/v2/SupportService/RefundPolicies | Create a new refund policy
[**delete_refund_policy_async**](RefundPoliciesApi.md#delete_refund_policy_async) | **DELETE** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Delete a refund policy
[**get_refund_policies_async**](RefundPoliciesApi.md#get_refund_policies_async) | **GET** /api/v2/SupportService/RefundPolicies | Retrieve a list of refund policies
[**get_refund_policies_count_async**](RefundPoliciesApi.md#get_refund_policies_count_async) | **GET** /api/v2/SupportService/RefundPolicies/Count | Get the count of refund policies
[**get_refund_policy_async**](RefundPoliciesApi.md#get_refund_policy_async) | **GET** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Retrieve a refund policy by ID
[**update_refund_policy_async**](RefundPoliciesApi.md#update_refund_policy_async) | **PUT** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Update a refund policy



## create_refund_policy_async

> models::EmptyEnvelope create_refund_policy_async(tenant_id, api_version, x_api_version, item_refund_policy_create_dto)
Create a new refund policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_refund_policy_create_dto** | Option<[**ItemRefundPolicyCreateDto**](ItemRefundPolicyCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_refund_policy_async

> models::EmptyEnvelope delete_refund_policy_async(tenant_id, refund_policy_id, api_version, x_api_version)
Delete a refund policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_policy_id** | **uuid::Uuid** |  | [required] |
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


## get_refund_policies_async

> models::ItemRefundPolicyDtoListEnvelope get_refund_policies_async(tenant_id, api_version, x_api_version)
Retrieve a list of refund policies

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_refund_policies_count_async

> models::Int32Envelope get_refund_policies_count_async(tenant_id, api_version, x_api_version)
Get the count of refund policies

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


## get_refund_policy_async

> models::ItemRefundPolicyDtoEnvelope get_refund_policy_async(tenant_id, refund_policy_id, api_version, x_api_version)
Retrieve a refund policy by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_policy_id** | **uuid::Uuid** |  | [required] |
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


## update_refund_policy_async

> models::EmptyEnvelope update_refund_policy_async(tenant_id, refund_policy_id, api_version, x_api_version, item_refund_policy_update_dto)
Update a refund policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**refund_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_refund_policy_update_dto** | Option<[**ItemRefundPolicyUpdateDto**](ItemRefundPolicyUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

