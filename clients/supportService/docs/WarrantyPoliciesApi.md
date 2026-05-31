# \WarrantyPoliciesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_warranty_policy_async**](WarrantyPoliciesApi.md#create_warranty_policy_async) | **POST** /api/v2/SupportService/WarrantyPolicies | Create a new warranty policy
[**delete_warranty_policy_async**](WarrantyPoliciesApi.md#delete_warranty_policy_async) | **DELETE** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Delete a warranty policy
[**get_warranty_policies_async**](WarrantyPoliciesApi.md#get_warranty_policies_async) | **GET** /api/v2/SupportService/WarrantyPolicies | Retrieve a list of warranty policies
[**get_warranty_policies_count_async**](WarrantyPoliciesApi.md#get_warranty_policies_count_async) | **GET** /api/v2/SupportService/WarrantyPolicies/Count | Get the count of warranty policies
[**get_warranty_policy_async**](WarrantyPoliciesApi.md#get_warranty_policy_async) | **GET** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Retrieve a warranty policy by ID
[**update_warranty_policy_async**](WarrantyPoliciesApi.md#update_warranty_policy_async) | **PUT** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Update a warranty policy



## create_warranty_policy_async

> models::EmptyEnvelope create_warranty_policy_async(tenant_id, api_version, x_api_version, item_warranty_policy_create_dto)
Create a new warranty policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_warranty_policy_create_dto** | Option<[**ItemWarrantyPolicyCreateDto**](ItemWarrantyPolicyCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_warranty_policy_async

> models::EmptyEnvelope delete_warranty_policy_async(tenant_id, warranty_policy_id, api_version, x_api_version)
Delete a warranty policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warranty_policy_id** | **uuid::Uuid** |  | [required] |
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


## get_warranty_policies_async

> models::ItemWarrantyPolicyDtoListEnvelope get_warranty_policies_async(tenant_id, api_version, x_api_version)
Retrieve a list of warranty policies

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_warranty_policies_count_async

> models::Int32Envelope get_warranty_policies_count_async(tenant_id, api_version, x_api_version)
Get the count of warranty policies

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


## get_warranty_policy_async

> models::ItemWarrantyPolicyDtoEnvelope get_warranty_policy_async(tenant_id, warranty_policy_id, api_version, x_api_version)
Retrieve a warranty policy by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warranty_policy_id** | **uuid::Uuid** |  | [required] |
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


## update_warranty_policy_async

> models::EmptyEnvelope update_warranty_policy_async(tenant_id, warranty_policy_id, api_version, x_api_version, item_warranty_policy_update_dto)
Update a warranty policy

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warranty_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_warranty_policy_update_dto** | Option<[**ItemWarrantyPolicyUpdateDto**](ItemWarrantyPolicyUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

