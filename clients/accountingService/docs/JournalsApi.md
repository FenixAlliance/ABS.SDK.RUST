# \JournalsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aggregate_journal_entry_credits_async**](JournalsApi.md#aggregate_journal_entry_credits_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Aggregate/Credits | Aggregate journal entry credits
[**aggregate_journal_entry_debits_async**](JournalsApi.md#aggregate_journal_entry_debits_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Aggregate/Debits | Aggregate journal entry debits
[**count_journals_async**](JournalsApi.md#count_journals_async) | **GET** /api/v2/AccountingService/Journals/Count | Count journals
[**create_journal_async**](JournalsApi.md#create_journal_async) | **POST** /api/v2/AccountingService/Journals | Create journal
[**create_journal_entry_async**](JournalsApi.md#create_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries | Create journal entry
[**delete_journal_async**](JournalsApi.md#delete_journal_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId} | Delete journal
[**delete_journal_entry_async**](JournalsApi.md#delete_journal_entry_async) | **DELETE** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Delete journal entry
[**get_journal_details_async**](JournalsApi.md#get_journal_details_async) | **GET** /api/v2/AccountingService/Journals/{journalId} | Get journal by ID
[**get_journal_entries_async**](JournalsApi.md#get_journal_entries_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries | Get journal entries
[**get_journal_entries_count_async**](JournalsApi.md#get_journal_entries_count_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/Count | Count journal entries
[**get_journal_entry_details_async**](JournalsApi.md#get_journal_entry_details_async) | **GET** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Get journal entry by ID
[**get_journals_async**](JournalsApi.md#get_journals_async) | **GET** /api/v2/AccountingService/Journals | Get all journals
[**patch_journal_async**](JournalsApi.md#patch_journal_async) | **PATCH** /api/v2/AccountingService/Journals/{journalId} | Patch a journal
[**patch_journal_entry_async**](JournalsApi.md#patch_journal_entry_async) | **PATCH** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Patch a journal entry
[**post_journal_entry_async**](JournalsApi.md#post_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId}/Post | Post a draft journal entry
[**reverse_journal_entry_async**](JournalsApi.md#reverse_journal_entry_async) | **POST** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId}/Reverse | Reverse a posted journal entry
[**update_journal_async**](JournalsApi.md#update_journal_async) | **PUT** /api/v2/AccountingService/Journals/{journalId} | Update journal
[**update_journal_entry_async**](JournalsApi.md#update_journal_entry_async) | **PUT** /api/v2/AccountingService/Journals/{journalId}/Entries/{entryId} | Update journal entry



## aggregate_journal_entry_credits_async

> models::MoneyEnvelope aggregate_journal_entry_credits_async(tenant_id, journal_id, currency_id, api_version, x_api_version)
Aggregate journal entry credits

Returns the sum of all credit amounts for entries in the specified journal, normalized to the target currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## aggregate_journal_entry_debits_async

> models::MoneyEnvelope aggregate_journal_entry_debits_async(tenant_id, journal_id, currency_id, api_version, x_api_version)
Aggregate journal entry debits

Returns the sum of all debit amounts for entries in the specified journal, normalized to the target currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_journals_async

> models::Int32Envelope count_journals_async(tenant_id, api_version, x_api_version)
Count journals

Returns the count of journals for the tenant.

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


## create_journal_async

> models::EmptyEnvelope create_journal_async(tenant_id, api_version, x_api_version, journal_create_dto)
Create journal

Creates a new journal for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_create_dto** | Option<[**JournalCreateDto**](JournalCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_journal_entry_async

> models::EmptyEnvelope create_journal_entry_async(tenant_id, journal_id, api_version, x_api_version, journal_entry_create_dto)
Create journal entry

Creates a new journal entry for a given journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_entry_create_dto** | Option<[**JournalEntryCreateDto**](JournalEntryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_journal_async

> models::EmptyEnvelope delete_journal_async(tenant_id, journal_id, api_version, x_api_version)
Delete journal

Deletes a journal by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
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


## delete_journal_entry_async

> models::EmptyEnvelope delete_journal_entry_async(tenant_id, journal_id, entry_id, api_version, x_api_version)
Delete journal entry

Deletes a specific journal entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
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


## get_journal_details_async

> models::JournalDtoEnvelope get_journal_details_async(tenant_id, journal_id, api_version, x_api_version)
Get journal by ID

Retrieves the details of a journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalDtoEnvelope**](JournalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_journal_entries_async

> models::JournalEntryDtoIReadOnlyListEnvelope get_journal_entries_async(tenant_id, journal_id, api_version, x_api_version)
Get journal entries

Gets entries for the specified journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalEntryDtoIReadOnlyListEnvelope**](JournalEntryDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_journal_entries_count_async

> models::Int32Envelope get_journal_entries_count_async(tenant_id, journal_id, api_version, x_api_version)
Count journal entries

Returns the number of entries in the specified journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
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


## get_journal_entry_details_async

> models::JournalEntryDtoEnvelope get_journal_entry_details_async(tenant_id, journal_id, entry_id, api_version, x_api_version)
Get journal entry by ID

Retrieves a single journal entry WITH its hydrated posting lines — each line's account, direction, description and currency facets (transaction / functional / account / USD).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalEntryDtoEnvelope**](JournalEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_journals_async

> models::JournalDtoIReadOnlyListEnvelope get_journals_async(tenant_id, api_version, x_api_version)
Get all journals

Retrieves all journals for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalDtoIReadOnlyListEnvelope**](JournalDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_journal_async

> models::EmptyEnvelope patch_journal_async(tenant_id, journal_id, api_version, x_api_version, operation)
Patch a journal

Partially updates a journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
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


## patch_journal_entry_async

> models::EmptyEnvelope patch_journal_entry_async(tenant_id, journal_id, entry_id, api_version, x_api_version, operation)
Patch a journal entry

Partially updates a journal entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
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


## post_journal_entry_async

> models::EmptyEnvelope post_journal_entry_async(tenant_id, journal_id, entry_id, api_version, x_api_version)
Post a draft journal entry

Posts a DRAFT journal entry into its own open fiscal period. Enforces the balanced-entry invariant and the open-period gate, then seals the entry (immutable — correct via reversal, never edit/delete). An unbalanced draft or a closed period is rejected. Requires the journals_post permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
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


## reverse_journal_entry_async

> models::EmptyEnvelope reverse_journal_entry_async(tenant_id, journal_id, entry_id, api_version, x_api_version, reverse_journal_entry_request)
Reverse a posted journal entry

Reverses a POSTED journal entry by writing a balanced compensating counter-entry into the supplied open fiscal period and marking the original Reversed — one atomic operation (append-only audit trail). Requires the journals_reverse permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**reverse_journal_entry_request** | Option<[**ReverseJournalEntryRequest**](ReverseJournalEntryRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_journal_async

> models::EmptyEnvelope update_journal_async(tenant_id, journal_id, api_version, x_api_version, journal_update_dto)
Update journal

Updates an existing journal.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_update_dto** | Option<[**JournalUpdateDto**](JournalUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_journal_entry_async

> models::EmptyEnvelope update_journal_entry_async(tenant_id, journal_id, entry_id, api_version, x_api_version, journal_entry_update_dto)
Update journal entry

Updates a specific journal entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_entry_update_dto** | Option<[**JournalEntryUpdateDto**](JournalEntryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

