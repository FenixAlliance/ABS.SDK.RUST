# \TaxPoliciesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_applied_tax_policy_record**](TaxPoliciesApi.md#create_applied_tax_policy_record) | **POST** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords | Create an applied tax policy record
[**create_item_tax_policy_record**](TaxPoliciesApi.md#create_item_tax_policy_record) | **POST** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords | Create an item tax policy record
[**create_tax_policy**](TaxPoliciesApi.md#create_tax_policy) | **POST** /api/v2/AccountingService/TaxPolicies | Create a tax policy
[**delete_applied_tax_policy_record**](TaxPoliciesApi.md#delete_applied_tax_policy_record) | **DELETE** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Delete an applied tax policy record
[**delete_item_tax_policy_record**](TaxPoliciesApi.md#delete_item_tax_policy_record) | **DELETE** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Delete an item tax policy record
[**delete_tax_policy**](TaxPoliciesApi.md#delete_tax_policy) | **DELETE** /api/v2/AccountingService/TaxPolicies/{id} | Delete a tax policy
[**get_applied_tax_policy_record**](TaxPoliciesApi.md#get_applied_tax_policy_record) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Get applied tax policy record by ID
[**get_applied_tax_policy_records**](TaxPoliciesApi.md#get_applied_tax_policy_records) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords | Get applied tax policy records
[**get_applied_tax_policy_records_count**](TaxPoliciesApi.md#get_applied_tax_policy_records_count) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/Count | Get applied tax policy records count
[**get_item_tax_policy_record**](TaxPoliciesApi.md#get_item_tax_policy_record) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Get item tax policy record by ID
[**get_item_tax_policy_records**](TaxPoliciesApi.md#get_item_tax_policy_records) | **GET** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords | Get item tax policy records
[**get_tax_policies**](TaxPoliciesApi.md#get_tax_policies) | **GET** /api/v2/AccountingService/TaxPolicies | Get all tax policies for a tenant
[**get_tax_policies_by_authority**](TaxPoliciesApi.md#get_tax_policies_by_authority) | **GET** /api/v2/AccountingService/TaxPolicies/ByAuthority/{authorityId} | Get tax policies by fiscal authority
[**get_tax_policies_count**](TaxPoliciesApi.md#get_tax_policies_count) | **GET** /api/v2/AccountingService/TaxPolicies/Count | Get tax policies count
[**get_tax_policy**](TaxPoliciesApi.md#get_tax_policy) | **GET** /api/v2/AccountingService/TaxPolicies/{id} | Get tax policy by ID
[**update_applied_tax_policy_record**](TaxPoliciesApi.md#update_applied_tax_policy_record) | **PUT** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/AppliedTaxPolicyRecords/{appliedTaxPolicyRecordId} | Update an applied tax policy record
[**update_item_tax_policy_record**](TaxPoliciesApi.md#update_item_tax_policy_record) | **PUT** /api/v2/AccountingService/TaxPolicies/{taxPolicyId}/ItemTaxPolicyRecords/{itemTaxPolicyRecordId} | Update an item tax policy record
[**update_tax_policy**](TaxPoliciesApi.md#update_tax_policy) | **PUT** /api/v2/AccountingService/TaxPolicies/{id} | Update a tax policy



## create_applied_tax_policy_record

> models::EmptyEnvelope create_applied_tax_policy_record(tenant_id, tax_policy_id, api_version, x_api_version, applied_tax_policy_record_create_dto)
Create an applied tax policy record

Creates a new applied tax policy record for the specified tax policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**applied_tax_policy_record_create_dto** | Option<[**AppliedTaxPolicyRecordCreateDto**](AppliedTaxPolicyRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_item_tax_policy_record

> models::EmptyEnvelope create_item_tax_policy_record(tenant_id, tax_policy_id, api_version, x_api_version, item_tax_policy_record_create_dto)
Create an item tax policy record

Creates a new item tax policy record for the specified tax policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_tax_policy_record_create_dto** | Option<[**ItemTaxPolicyRecordCreateDto**](ItemTaxPolicyRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tax_policy

> models::EmptyEnvelope create_tax_policy(tenant_id, api_version, x_api_version, tax_policy_create_dto)
Create a tax policy

Creates a new tax policy for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_policy_create_dto** | Option<[**TaxPolicyCreateDto**](TaxPolicyCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_applied_tax_policy_record

> models::EmptyEnvelope delete_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, api_version, x_api_version)
Delete an applied tax policy record

Deletes an applied tax policy record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**applied_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
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


## delete_item_tax_policy_record

> models::EmptyEnvelope delete_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, api_version, x_api_version)
Delete an item tax policy record

Deletes an item tax policy record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
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


## delete_tax_policy

> models::EmptyEnvelope delete_tax_policy(tenant_id, id, api_version, x_api_version)
Delete a tax policy

Deletes a tax policy identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_applied_tax_policy_record

> models::AppliedTaxPolicyRecordDtoEnvelope get_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, api_version, x_api_version)
Get applied tax policy record by ID

Retrieves a specific applied tax policy record by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**applied_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppliedTaxPolicyRecordDtoEnvelope**](AppliedTaxPolicyRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_applied_tax_policy_records

> models::AppliedTaxPolicyRecordDtoListEnvelope get_applied_tax_policy_records(tenant_id, tax_policy_id, api_version, x_api_version)
Get applied tax policy records

Retrieves all applied tax policy records for the specified tax policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppliedTaxPolicyRecordDtoListEnvelope**](AppliedTaxPolicyRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_applied_tax_policy_records_count

> models::Int32Envelope get_applied_tax_policy_records_count(tenant_id, tax_policy_id, api_version, x_api_version)
Get applied tax policy records count

Returns the total count of applied tax policy records for the specified tax policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
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


## get_item_tax_policy_record

> models::ItemTaxPolicyRecordDtoEnvelope get_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, api_version, x_api_version)
Get item tax policy record by ID

Retrieves a specific item tax policy record by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyRecordDtoEnvelope**](ItemTaxPolicyRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_tax_policy_records

> models::ItemTaxPolicyRecordDtoListEnvelope get_item_tax_policy_records(tenant_id, tax_policy_id, api_version, x_api_version)
Get item tax policy records

Retrieves all item tax policy records for the specified tax policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyRecordDtoListEnvelope**](ItemTaxPolicyRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_policies

> models::TaxPolicyDtoListEnvelope get_tax_policies(tenant_id, api_version, x_api_version)
Get all tax policies for a tenant

Retrieves all tax policies for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxPolicyDtoListEnvelope**](TaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_policies_by_authority

> models::TaxPolicyDtoListEnvelope get_tax_policies_by_authority(tenant_id, authority_id, api_version, x_api_version)
Get tax policies by fiscal authority

Retrieves all tax policies associated with the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxPolicyDtoListEnvelope**](TaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_policies_count

> models::Int32Envelope get_tax_policies_count(tenant_id, api_version, x_api_version)
Get tax policies count

Returns the count of tax policies for the specified tenant.

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


## get_tax_policy

> models::TaxPolicyDtoEnvelope get_tax_policy(tenant_id, id, api_version, x_api_version)
Get tax policy by ID

Retrieves a specific tax policy by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxPolicyDtoEnvelope**](TaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_applied_tax_policy_record

> models::EmptyEnvelope update_applied_tax_policy_record(tenant_id, tax_policy_id, applied_tax_policy_record_id, api_version, x_api_version, applied_tax_policy_record_update_dto)
Update an applied tax policy record

Updates an existing applied tax policy record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**applied_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**applied_tax_policy_record_update_dto** | Option<[**AppliedTaxPolicyRecordUpdateDto**](AppliedTaxPolicyRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_tax_policy_record

> models::EmptyEnvelope update_item_tax_policy_record(tenant_id, tax_policy_id, item_tax_policy_record_id, api_version, x_api_version, item_tax_policy_record_update_dto)
Update an item tax policy record

Updates an existing item tax policy record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tax_policy_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_tax_policy_record_update_dto** | Option<[**ItemTaxPolicyRecordUpdateDto**](ItemTaxPolicyRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tax_policy

> models::EmptyEnvelope update_tax_policy(tenant_id, id, api_version, x_api_version, tax_policy_update_dto)
Update a tax policy

Updates an existing tax policy identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_policy_update_dto** | Option<[**TaxPolicyUpdateDto**](TaxPolicyUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

