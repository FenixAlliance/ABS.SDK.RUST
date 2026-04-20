# \FiscalResponsibilityRecordsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#create_fiscal_responsibility_record) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords | Create a fiscal responsibility record
[**delete_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#delete_fiscal_responsibility_record) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Delete a fiscal responsibility record
[**get_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_record) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Get fiscal responsibility record by ID
[**get_fiscal_responsibility_records**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_records) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords | Get fiscal responsibility records
[**get_fiscal_responsibility_records_count**](FiscalResponsibilityRecordsApi.md#get_fiscal_responsibility_records_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId}/FiscalResponsibilityRecords/Count | Get fiscal responsibility records count
[**update_fiscal_responsibility_record**](FiscalResponsibilityRecordsApi.md#update_fiscal_responsibility_record) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilityRecords/{fiscalResponsibilityRecordId} | Update a fiscal responsibility record



## create_fiscal_responsibility_record

> models::EmptyEnvelope create_fiscal_responsibility_record(tenant_id, api_version, x_api_version, fiscal_responsibility_record_create_dto)
Create a fiscal responsibility record

Creates a new fiscal responsibility record for a fiscal responsibility.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_responsibility_record_create_dto** | Option<[**FiscalResponsibilityRecordCreateDto**](FiscalResponsibilityRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_responsibility_record

> models::EmptyEnvelope delete_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, api_version, x_api_version)
Delete a fiscal responsibility record

Deletes a fiscal responsibility record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_responsibility_record_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_responsibility_record

> models::FiscalResponsibilityRecordDtoEnvelope get_fiscal_responsibility_record(tenant_id, fiscal_authority_id, fiscal_responsibility_id, fiscal_responsibility_record_id, api_version, x_api_version)
Get fiscal responsibility record by ID

Retrieves a specific fiscal responsibility record by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
**fiscal_responsibility_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalResponsibilityRecordDtoEnvelope**](FiscalResponsibilityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_responsibility_records

> models::FiscalResponsibilityRecordDtoListEnvelope get_fiscal_responsibility_records(tenant_id, fiscal_authority_id, fiscal_responsibility_id, api_version, x_api_version)
Get fiscal responsibility records

Retrieves all fiscal responsibility records for the specified fiscal responsibility.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalResponsibilityRecordDtoListEnvelope**](FiscalResponsibilityRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_responsibility_records_count

> models::Int32Envelope get_fiscal_responsibility_records_count(tenant_id, fiscal_authority_id, fiscal_responsibility_id, api_version, x_api_version)
Get fiscal responsibility records count

Returns the total count of fiscal responsibility records for the specified fiscal responsibility.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
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


## update_fiscal_responsibility_record

> models::EmptyEnvelope update_fiscal_responsibility_record(tenant_id, fiscal_responsibility_record_id, api_version, x_api_version, fiscal_responsibility_record_update_dto)
Update a fiscal responsibility record

Updates an existing fiscal responsibility record identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_responsibility_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_responsibility_record_update_dto** | Option<[**FiscalResponsibilityRecordUpdateDto**](FiscalResponsibilityRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

