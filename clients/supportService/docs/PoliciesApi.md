# \PoliciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_refund_policy_async**](PoliciesApi.md#create_refund_policy_async) | **POST** /api/v2/SupportService/RefundPolicies | Create a new refund policy
[**create_return_policy_async**](PoliciesApi.md#create_return_policy_async) | **POST** /api/v2/SupportService/ReturnPolicies | Create a new return policy
[**create_warranty_policy_async**](PoliciesApi.md#create_warranty_policy_async) | **POST** /api/v2/SupportService/WarrantyPolicies | Create a new warranty policy
[**delete_refund_policy_async**](PoliciesApi.md#delete_refund_policy_async) | **DELETE** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Delete a refund policy
[**delete_return_policy_async**](PoliciesApi.md#delete_return_policy_async) | **DELETE** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Delete a return policy
[**delete_warranty_policy_async**](PoliciesApi.md#delete_warranty_policy_async) | **DELETE** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Delete a warranty policy
[**get_refund_policies_async**](PoliciesApi.md#get_refund_policies_async) | **GET** /api/v2/SupportService/RefundPolicies | Retrieve a list of refund policies
[**get_refund_policies_count_async**](PoliciesApi.md#get_refund_policies_count_async) | **GET** /api/v2/SupportService/RefundPolicies/Count | Get the count of refund policies
[**get_refund_policy_async**](PoliciesApi.md#get_refund_policy_async) | **GET** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Retrieve a refund policy by ID
[**get_return_policies_async**](PoliciesApi.md#get_return_policies_async) | **GET** /api/v2/SupportService/ReturnPolicies | Retrieve a list of return policies
[**get_return_policies_count_async**](PoliciesApi.md#get_return_policies_count_async) | **GET** /api/v2/SupportService/ReturnPolicies/Count | Get the count of return policies
[**get_return_policy_async**](PoliciesApi.md#get_return_policy_async) | **GET** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Retrieve a return policy by ID
[**get_warranty_policies_async**](PoliciesApi.md#get_warranty_policies_async) | **GET** /api/v2/SupportService/WarrantyPolicies | Retrieve a list of warranty policies
[**get_warranty_policies_count_async**](PoliciesApi.md#get_warranty_policies_count_async) | **GET** /api/v2/SupportService/WarrantyPolicies/Count | Get the count of warranty policies
[**get_warranty_policy_async**](PoliciesApi.md#get_warranty_policy_async) | **GET** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Retrieve a warranty policy by ID
[**update_refund_policy_async**](PoliciesApi.md#update_refund_policy_async) | **PUT** /api/v2/SupportService/RefundPolicies/{refundPolicyId} | Update a refund policy
[**update_return_policy_async**](PoliciesApi.md#update_return_policy_async) | **PUT** /api/v2/SupportService/ReturnPolicies/{returnPolicyId} | Update a return policy
[**update_warranty_policy_async**](PoliciesApi.md#update_warranty_policy_async) | **PUT** /api/v2/SupportService/WarrantyPolicies/{warrantyPolicyId} | Update a warranty policy



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

