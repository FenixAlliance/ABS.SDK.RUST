# \AccountsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**balance_account_async**](AccountsApi.md#balance_account_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Balance | Balance account
[**balance_root_account_async**](AccountsApi.md#balance_root_account_async) | **POST** /api/v2/AccountingService/Accounts/Root/Balance | Balance root account
[**create_account_async**](AccountsApi.md#create_account_async) | **POST** /api/v2/AccountingService/Accounts | Get root accounts
[**create_account_credit_async**](AccountsApi.md#create_account_credit_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Credits | Create account credit
[**create_account_debit_async**](AccountsApi.md#create_account_debit_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Debits | Create account debit
[**create_account_entry_async**](AccountsApi.md#create_account_entry_async) | **POST** /api/v2/AccountingService/Accounts/{accountId}/Entries | Create account entry
[**create_account_relation_async**](AccountsApi.md#create_account_relation_async) | **POST** /api/v2/AccountingService/Accounts/Relations | Create account relation
[**create_account_type_async**](AccountsApi.md#create_account_type_async) | **POST** /api/v2/AccountingService/Accounts/Types | Create account type
[**delete_account_async**](AccountsApi.md#delete_account_async) | **DELETE** /api/v2/AccountingService/Accounts/{accountId} | Delete an account
[**delete_account_entry_async**](AccountsApi.md#delete_account_entry_async) | **DELETE** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Delete account entry
[**delete_account_relation_async**](AccountsApi.md#delete_account_relation_async) | **DELETE** /api/v2/AccountingService/Accounts/Relations/{accountRelationId} | Delete account relation
[**delete_account_type_async**](AccountsApi.md#delete_account_type_async) | **DELETE** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Delete account type
[**get_account_aggregate_async**](AccountsApi.md#get_account_aggregate_async) | **POST** /api/v2/AccountingService/Accounts/Aggregate | Get account aggregate
[**get_account_credits_async**](AccountsApi.md#get_account_credits_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Credits | Get account credits
[**get_account_credits_count_async**](AccountsApi.md#get_account_credits_count_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Credits/Count | Get account credits count
[**get_account_debits_async**](AccountsApi.md#get_account_debits_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Debits | Get account debits
[**get_account_debits_count_async**](AccountsApi.md#get_account_debits_count_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Debits/Count | Get account debits count
[**get_account_details_async**](AccountsApi.md#get_account_details_async) | **GET** /api/v2/AccountingService/Accounts/{accountId} | Get account details
[**get_account_entries_async**](AccountsApi.md#get_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries | Get account entries
[**get_account_entry_async**](AccountsApi.md#get_account_entry_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Get account entry
[**get_account_relations_async**](AccountsApi.md#get_account_relations_async) | **GET** /api/v2/AccountingService/Accounts/Relations | Get account relations
[**get_account_relations_count_async**](AccountsApi.md#get_account_relations_count_async) | **GET** /api/v2/AccountingService/Accounts/Relations/Count | Get account relations count
[**get_account_types_async**](AccountsApi.md#get_account_types_async) | **GET** /api/v2/AccountingService/Accounts/Types | Get account types
[**get_account_types_count_async**](AccountsApi.md#get_account_types_count_async) | **GET** /api/v2/AccountingService/Accounts/Types/Count | Get account types count
[**get_accounts_async**](AccountsApi.md#get_accounts_async) | **GET** /api/v2/AccountingService/Accounts | Creates a new account
[**get_accounts_count_async**](AccountsApi.md#get_accounts_count_async) | **GET** /api/v2/AccountingService/Accounts/Count | Get the number of accounts
[**get_child_accounts_async**](AccountsApi.md#get_child_accounts_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Children | Get child accounts
[**get_credit_account_entries_async**](AccountsApi.md#get_credit_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/Credit | Get credit account entries
[**get_debit_account_entries_async**](AccountsApi.md#get_debit_account_entries_async) | **GET** /api/v2/AccountingService/Accounts/{accountId}/Entries/Debit | Get debit account entries
[**get_root_accounts_async**](AccountsApi.md#get_root_accounts_async) | **GET** /api/v2/AccountingService/Accounts/Root | Get root accounts
[**patch_account_async**](AccountsApi.md#patch_account_async) | **PATCH** /api/v2/AccountingService/Accounts/{accountId} | Patch an account
[**update_account_async**](AccountsApi.md#update_account_async) | **PUT** /api/v2/AccountingService/Accounts/{accountId} | Update an account
[**update_account_entry_async**](AccountsApi.md#update_account_entry_async) | **PUT** /api/v2/AccountingService/Accounts/{accountId}/Entries/{entryId} | Update account entry
[**update_account_relation_async**](AccountsApi.md#update_account_relation_async) | **PUT** /api/v2/AccountingService/Accounts/Relations/{accountRelationId} | Update account relation
[**update_account_type_async**](AccountsApi.md#update_account_type_async) | **PUT** /api/v2/AccountingService/Accounts/Types/{accountTypeId} | Update account type



## balance_account_async

> models::AccountDtoEnvelope balance_account_async(tenant_id, account_id, api_version, x_api_version)
Balance account

Balance account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## balance_root_account_async

> models::AccountDtoListEnvelope balance_root_account_async(tenant_id, api_version, x_api_version)
Balance root account

Balance root account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_async

> models::AccountDtoListEnvelope create_account_async(tenant_id, api_version, x_api_version, account_create_dto)
Get root accounts

Get root accounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_create_dto** | Option<[**AccountCreateDto**](AccountCreateDto.md)> |  |  |

### Return type

[**models::AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_credit_async

> models::AccountingEntryDtoListEnvelope create_account_credit_async(tenant_id, account_id, api_version, x_api_version, accounting_entry_create_dto)
Create account credit

Create account credit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_entry_create_dto** | Option<[**AccountingEntryCreateDto**](AccountingEntryCreateDto.md)> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_debit_async

> models::AccountingEntryDtoListEnvelope create_account_debit_async(tenant_id, account_id, api_version, x_api_version, accounting_entry_create_dto)
Create account debit

Create account debit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_entry_create_dto** | Option<[**AccountingEntryCreateDto**](AccountingEntryCreateDto.md)> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_entry_async

> models::AccountingEntryDtoEnvelope create_account_entry_async(tenant_id, account_id, api_version, x_api_version, accounting_entry_create_dto)
Create account entry

Create account entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_entry_create_dto** | Option<[**AccountingEntryCreateDto**](AccountingEntryCreateDto.md)> |  |  |

### Return type

[**models::AccountingEntryDtoEnvelope**](AccountingEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_relation_async

> models::EmptyEnvelope create_account_relation_async(tenant_id, account_id, api_version, x_api_version, account_relation_create_dto)
Create account relation

Create account relation.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_relation_create_dto** | Option<[**AccountRelationCreateDto**](AccountRelationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_type_async

> models::EmptyEnvelope create_account_type_async(tenant_id, account_id, api_version, x_api_version, account_type_create_dto)
Create account type

Create account type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_type_create_dto** | Option<[**AccountTypeCreateDto**](AccountTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_account_async

> models::EmptyEnvelope delete_account_async(tenant_id, account_id, api_version, x_api_version)
Delete an account

Delete an account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## delete_account_entry_async

> models::EmptyEnvelope delete_account_entry_async(tenant_id, account_id, entry_id, api_version, x_api_version)
Delete account entry

Delete account entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
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


## delete_account_relation_async

> models::EmptyEnvelope delete_account_relation_async(tenant_id, account_relation_id, account_id, api_version, x_api_version)
Delete account relation

Delete account relation.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_relation_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## delete_account_type_async

> models::EmptyEnvelope delete_account_type_async(tenant_id, account_type_id, account_id, api_version, x_api_version)
Delete account type

Delete account type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_type_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## get_account_aggregate_async

> models::AccountingEntryDtoListEnvelope get_account_aggregate_async(tenant_id, currency_id, api_version, x_api_version, account_dto)
Get account aggregate

Get account aggregate.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_dto** | Option<[**Vec<models::AccountDto>**](AccountDto.md)> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_credits_async

> models::AccountingEntryDtoListEnvelope get_account_credits_async(tenant_id, account_id, api_version, x_api_version)
Get account credits

Get account credits.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_credits_count_async

> models::Int32Envelope get_account_credits_count_async(tenant_id, account_id, api_version, x_api_version)
Get account credits count

Get account credits count.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## get_account_debits_async

> models::AccountingEntryDtoListEnvelope get_account_debits_async(tenant_id, account_id, api_version, x_api_version)
Get account debits

Get account debits.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_debits_count_async

> models::Int32Envelope get_account_debits_count_async(tenant_id, account_id, api_version, x_api_version)
Get account debits count

Get account debits count.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## get_account_details_async

> models::AccountDtoEnvelope get_account_details_async(tenant_id, account_id, api_version, x_api_version)
Get account details

Get account details.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_entries_async

> models::AccountingEntryDtoListEnvelope get_account_entries_async(tenant_id, account_id, api_version, x_api_version)
Get account entries

Get account entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_entry_async

> models::AccountingEntryDtoEnvelope get_account_entry_async(tenant_id, account_id, entry_id, api_version, x_api_version)
Get account entry

Get account entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoEnvelope**](AccountingEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_relations_async

> models::AccountRelationDtoListEnvelope get_account_relations_async(tenant_id, account_id, api_version, x_api_version)
Get account relations

Get account relations.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountRelationDtoListEnvelope**](AccountRelationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_relations_count_async

> models::Int32Envelope get_account_relations_count_async(tenant_id, account_id, api_version, x_api_version)
Get account relations count

Get account relations count.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
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


## get_account_types_async

> models::AccountTypeDtoListEnvelope get_account_types_async(tenant_id, account_type_id, api_version, x_api_version)
Get account types

Get account types.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountTypeDtoListEnvelope**](AccountTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_types_count_async

> models::Int32Envelope get_account_types_count_async(tenant_id, account_type_id, api_version, x_api_version)
Get account types count

Get account types count.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_type_id** | **uuid::Uuid** |  | [required] |
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


## get_accounts_async

> models::AccountDtoListEnvelope get_accounts_async(tenant_id, api_version, x_api_version)
Creates a new account

Creates a new account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_accounts_count_async

> models::Int32Envelope get_accounts_count_async(tenant_id, api_version, x_api_version)
Get the number of accounts

Get the number of accounts.

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


## get_child_accounts_async

> models::AccountDtoListEnvelope get_child_accounts_async(tenant_id, account_id, api_version, x_api_version)
Get child accounts

Get child accounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_credit_account_entries_async

> models::AccountingEntryDtoListEnvelope get_credit_account_entries_async(tenant_id, account_id, api_version, x_api_version)
Get credit account entries

Get credit account entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_debit_account_entries_async

> models::AccountingEntryDtoListEnvelope get_debit_account_entries_async(tenant_id, account_id, api_version, x_api_version)
Get debit account entries

Get debit account entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountingEntryDtoListEnvelope**](AccountingEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_root_accounts_async

> models::AccountDtoListEnvelope get_root_accounts_async(tenant_id, api_version, x_api_version)
Get root accounts

Get root accounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountDtoListEnvelope**](AccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_account_async

> models::EmptyEnvelope patch_account_async(tenant_id, account_id, api_version, x_api_version, operation)
Patch an account

Patch an account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_async

> models::AccountDtoEnvelope update_account_async(tenant_id, account_id, api_version, x_api_version, account_update_dto)
Update an account

Update an account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_update_dto** | Option<[**AccountUpdateDto**](AccountUpdateDto.md)> |  |  |

### Return type

[**models::AccountDtoEnvelope**](AccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_entry_async

> models::EmptyEnvelope update_account_entry_async(tenant_id, account_id, entry_id, api_version, x_api_version, accounting_entry_update_dto)
Update account entry

Update account entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**accounting_entry_update_dto** | Option<[**AccountingEntryUpdateDto**](AccountingEntryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_relation_async

> models::EmptyEnvelope update_account_relation_async(tenant_id, account_relation_id, account_id, api_version, x_api_version, account_relation_update_dto)
Update account relation

Update account relation.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_relation_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_relation_update_dto** | Option<[**AccountRelationUpdateDto**](AccountRelationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_type_async

> models::EmptyEnvelope update_account_type_async(tenant_id, account_type_id, account_id, api_version, x_api_version, account_type_update_dto)
Update account type

Update account type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_type_id** | **uuid::Uuid** |  | [required] |
**account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_type_update_dto** | Option<[**AccountTypeUpdateDto**](AccountTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

