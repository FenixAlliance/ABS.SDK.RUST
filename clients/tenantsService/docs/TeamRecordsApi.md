# \TeamRecordsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_team_record**](TeamRecordsApi.md#create_tenant_team_record) | **POST** /api/v2/TenantsService/TeamRecords | Create a new tenant team record
[**delete_tenant_team_record**](TeamRecordsApi.md#delete_tenant_team_record) | **DELETE** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Delete a tenant team record
[**get_tenant_team_record_by_id**](TeamRecordsApi.md#get_tenant_team_record_by_id) | **GET** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Retrieve a single tenant team record by its ID
[**get_tenant_team_records**](TeamRecordsApi.md#get_tenant_team_records) | **GET** /api/v2/TenantsService/TeamRecords | Retrieve a list of tenant team records
[**get_tenant_team_records_count**](TeamRecordsApi.md#get_tenant_team_records_count) | **GET** /api/v2/TenantsService/TeamRecords/Count | Get the count of tenant team records
[**update_tenant_team_record**](TeamRecordsApi.md#update_tenant_team_record) | **PUT** /api/v2/TenantsService/TeamRecords/{tenantTeamRecordId} | Update a tenant team record



## create_tenant_team_record

> models::EmptyEnvelope create_tenant_team_record(tenant_id, api_version, x_api_version, tenant_team_record_create_dto)
Create a new tenant team record

Create a new tenant team record

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_team_record_create_dto** | Option<[**TenantTeamRecordCreateDto**](TenantTeamRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_team_record

> models::EmptyEnvelope delete_tenant_team_record(tenant_id, tenant_team_record_id, api_version, x_api_version)
Delete a tenant team record

Delete a tenant team record

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_record_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_team_record_by_id

> models::TenantTeamRecordDtoEnvelope get_tenant_team_record_by_id(tenant_id, tenant_team_record_id, api_version, x_api_version)
Retrieve a single tenant team record by its ID

Retrieve a single tenant team record by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTeamRecordDtoEnvelope**](TenantTeamRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_team_records

> models::TenantTeamRecordDtoListEnvelope get_tenant_team_records(tenant_id, api_version, x_api_version)
Retrieve a list of tenant team records

Retrieve a list of tenant team records

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTeamRecordDtoListEnvelope**](TenantTeamRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_team_records_count

> models::Int32Envelope get_tenant_team_records_count(tenant_id, api_version, x_api_version)
Get the count of tenant team records

Get the count of tenant team records

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


## update_tenant_team_record

> models::EmptyEnvelope update_tenant_team_record(tenant_id, tenant_team_record_id, api_version, x_api_version, tenant_team_record_update_dto)
Update a tenant team record

Update a tenant team record

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_team_record_update_dto** | Option<[**TenantTeamRecordUpdateDto**](TenantTeamRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

