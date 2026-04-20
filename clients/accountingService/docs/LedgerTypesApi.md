# \LedgerTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_ledger_type_async**](LedgerTypesApi.md#create_ledger_type_async) | **POST** /api/v2/AccountingService/LedgerTypes | Creates a new ledger type
[**delete_ledger_type_async**](LedgerTypesApi.md#delete_ledger_type_async) | **DELETE** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Deletes a ledger type
[**get_ledger_type_details_async**](LedgerTypesApi.md#get_ledger_type_details_async) | **GET** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Gets a ledger type by ID
[**get_ledger_types_async**](LedgerTypesApi.md#get_ledger_types_async) | **GET** /api/v2/AccountingService/LedgerTypes | Retrieves all ledger types
[**get_ledger_types_count_async**](LedgerTypesApi.md#get_ledger_types_count_async) | **GET** /api/v2/AccountingService/LedgerTypes/Count | Counts ledger types
[**update_ledger_type_async**](LedgerTypesApi.md#update_ledger_type_async) | **PUT** /api/v2/AccountingService/LedgerTypes/{ledgerTypeId} | Updates a ledger type



## create_ledger_type_async

> models::EmptyEnvelope create_ledger_type_async(tenant_id, api_version, x_api_version, ledger_type_create_dto)
Creates a new ledger type

Creates a new ledger type for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**ledger_type_create_dto** | Option<[**LedgerTypeCreateDto**](LedgerTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_ledger_type_async

> models::EmptyEnvelope delete_ledger_type_async(tenant_id, ledger_type_id, api_version, x_api_version)
Deletes a ledger type

Deletes the specified ledger type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**ledger_type_id** | **uuid::Uuid** |  | [required] |
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


## get_ledger_type_details_async

> models::LedgerTypeDtoEnvelope get_ledger_type_details_async(tenant_id, ledger_type_id, api_version, x_api_version)
Gets a ledger type by ID

Retrieves the details of a ledger type using its unique ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**ledger_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LedgerTypeDtoEnvelope**](LedgerTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_ledger_types_async

> models::LedgerTypeDtoIReadOnlyListEnvelope get_ledger_types_async(tenant_id, api_version, x_api_version)
Retrieves all ledger types

Gets all ledger types for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LedgerTypeDtoIReadOnlyListEnvelope**](LedgerTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_ledger_types_count_async

> models::Int32Envelope get_ledger_types_count_async(tenant_id, api_version, x_api_version)
Counts ledger types

Gets the count of ledger types for the current tenant.

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


## update_ledger_type_async

> models::EmptyEnvelope update_ledger_type_async(tenant_id, ledger_type_id, api_version, x_api_version, ledger_type_update_dto)
Updates a ledger type

Updates the specified ledger type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**ledger_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**ledger_type_update_dto** | Option<[**LedgerTypeUpdateDto**](LedgerTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

