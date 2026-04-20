# \JournalTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_journal_type_async**](JournalTypesApi.md#create_journal_type_async) | **POST** /api/v2/AccountingService/JournalTypes | Creates a new journal type
[**delete_journal_type_async**](JournalTypesApi.md#delete_journal_type_async) | **DELETE** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Deletes a journal type
[**get_journal_type_details_async**](JournalTypesApi.md#get_journal_type_details_async) | **GET** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Retrieves a journal type by ID
[**get_journal_types_async**](JournalTypesApi.md#get_journal_types_async) | **GET** /api/v2/AccountingService/JournalTypes | Retrieves all journal types
[**get_journal_types_count_async**](JournalTypesApi.md#get_journal_types_count_async) | **GET** /api/v2/AccountingService/JournalTypes/Count | Counts journal types
[**update_journal_type_async**](JournalTypesApi.md#update_journal_type_async) | **PUT** /api/v2/AccountingService/JournalTypes/{journalTypeId} | Updates an existing journal type



## create_journal_type_async

> models::EmptyEnvelope create_journal_type_async(tenant_id, api_version, x_api_version, journal_type_create_dto)
Creates a new journal type

Adds a new journal type to the tenant's catalog.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_type_create_dto** | Option<[**JournalTypeCreateDto**](JournalTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_journal_type_async

> models::EmptyEnvelope delete_journal_type_async(tenant_id, journal_type_id, api_version, x_api_version)
Deletes a journal type

Removes a journal type from the tenant's configuration.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_type_id** | **uuid::Uuid** |  | [required] |
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


## get_journal_type_details_async

> models::JournalTypeDtoEnvelope get_journal_type_details_async(tenant_id, journal_type_id, api_version, x_api_version)
Retrieves a journal type by ID

Fetches the journal type matching the specified ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalTypeDtoEnvelope**](JournalTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_journal_types_async

> models::JournalTypeDtoIReadOnlyListEnvelope get_journal_types_async(tenant_id, api_version, x_api_version)
Retrieves all journal types

Fetches all journal types for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JournalTypeDtoIReadOnlyListEnvelope**](JournalTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_journal_types_count_async

> models::Int32Envelope get_journal_types_count_async(tenant_id, api_version, x_api_version)
Counts journal types

Returns the total number of journal types available for the tenant.

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


## update_journal_type_async

> models::EmptyEnvelope update_journal_type_async(tenant_id, journal_type_id, api_version, x_api_version, journal_type_update_dto)
Updates an existing journal type

Modifies the details of a specific journal type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**journal_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**journal_type_update_dto** | Option<[**JournalTypeUpdateDto**](JournalTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

