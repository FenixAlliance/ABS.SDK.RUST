# \ReturnPoliciesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_return_policy_async**](ReturnPoliciesApi.md#create_return_policy_async) | **POST** /api/v2/SupportService/ReturnPolicies | Create a new return policy
[**delete_return_policy_async**](ReturnPoliciesApi.md#delete_return_policy_async) | **DELETE** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Delete a return policy
[**get_return_policies_async**](ReturnPoliciesApi.md#get_return_policies_async) | **GET** /api/v2/SupportService/ReturnPolicies | Retrieve a list of return policies
[**get_return_policies_count_async**](ReturnPoliciesApi.md#get_return_policies_count_async) | **GET** /api/v2/SupportService/ReturnPolicies/Count | Get the count of return policies
[**get_return_policy_async**](ReturnPoliciesApi.md#get_return_policy_async) | **GET** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Retrieve a return policy by ID
[**update_return_policy_async**](ReturnPoliciesApi.md#update_return_policy_async) | **PUT** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Update a return policy



## create_return_policy_async

> models::EmptyEnvelope create_return_policy_async(tenant_id, api_version, x_api_version, item_return_policy_create_dto)
Create a new return policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_return_policy_create_dto** | Option<[**ItemReturnPolicyCreateDto**](ItemReturnPolicyCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_return_policy_async

> models::EmptyEnvelope delete_return_policy_async(tenant_id, return_policy_id, api_version, x_api_version)
Delete a return policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_policy_id** | **uuid::Uuid** |  | [required] |
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


## get_return_policies_async

> models::ItemReturnPolicyDtoListEnvelope get_return_policies_async(tenant_id, api_version, x_api_version)
Retrieve a list of return policies

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_return_policies_count_async

> models::Int32Envelope get_return_policies_count_async(tenant_id, api_version, x_api_version)
Get the count of return policies

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


## get_return_policy_async

> models::ItemReturnPolicyDtoEnvelope get_return_policy_async(tenant_id, return_policy_id, api_version, x_api_version)
Retrieve a return policy by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_policy_id** | **uuid::Uuid** |  | [required] |
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


## update_return_policy_async

> models::EmptyEnvelope update_return_policy_async(tenant_id, return_policy_id, api_version, x_api_version, item_return_policy_update_dto)
Update a return policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_return_policy_update_dto** | Option<[**ItemReturnPolicyUpdateDto**](ItemReturnPolicyUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

