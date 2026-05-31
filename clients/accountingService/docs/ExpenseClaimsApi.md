# \ExpenseClaimsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_expense_claim**](ExpenseClaimsApi.md#create_expense_claim) | **POST** /api/v2/AccountingService/ExpenseClaims | Create an expense claim
[**delete_expense_claim**](ExpenseClaimsApi.md#delete_expense_claim) | **DELETE** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Delete an expense claim
[**get_expense_claim**](ExpenseClaimsApi.md#get_expense_claim) | **GET** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Get an expense claim by id
[**get_expense_claims**](ExpenseClaimsApi.md#get_expense_claims) | **GET** /api/v2/AccountingService/ExpenseClaims | Get all expense claims for a tenant
[**get_expense_claims_count**](ExpenseClaimsApi.md#get_expense_claims_count) | **GET** /api/v2/AccountingService/ExpenseClaims/Count | Get the count of expense claims for a tenant
[**update_expense_claim**](ExpenseClaimsApi.md#update_expense_claim) | **PUT** /api/v2/AccountingService/ExpenseClaims/{expenseClaimId} | Update an expense claim



## create_expense_claim

> models::EmptyEnvelope create_expense_claim(tenant_id, expense_claim_create_dto, api_version, x_api_version)
Create an expense claim

Creates a new expense claim.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_claim_create_dto** | [**ExpenseClaimCreateDto**](ExpenseClaimCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_expense_claim

> models::EmptyEnvelope delete_expense_claim(tenant_id, expense_claim_id, api_version, x_api_version)
Delete an expense claim

Deletes an expense claim.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_claim_id** | **uuid::Uuid** |  | [required] |
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


## get_expense_claim

> models::ExpenseClaimDtoEnvelope get_expense_claim(tenant_id, expense_claim_id, api_version, x_api_version)
Get an expense claim by id

Retrieves an expense claim by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_claim_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExpenseClaimDtoEnvelope**](ExpenseClaimDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_expense_claims

> models::ExpenseClaimDtoListEnvelope get_expense_claims(tenant_id, api_version, x_api_version)
Get all expense claims for a tenant

Retrieves all expense claims for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExpenseClaimDtoListEnvelope**](ExpenseClaimDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_expense_claims_count

> models::Int32Envelope get_expense_claims_count(tenant_id, api_version, x_api_version)
Get the count of expense claims for a tenant

Retrieves the count of expense claims for the specified tenant using OData query options.

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


## update_expense_claim

> models::EmptyEnvelope update_expense_claim(tenant_id, expense_claim_id, expense_claim_update_dto, api_version, x_api_version)
Update an expense claim

Updates an existing expense claim.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_claim_id** | **uuid::Uuid** |  | [required] |
**expense_claim_update_dto** | [**ExpenseClaimUpdateDto**](ExpenseClaimUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

