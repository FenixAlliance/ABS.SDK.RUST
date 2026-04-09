# \FiscalResponsibilitiesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_fiscal_responsibility**](FiscalResponsibilitiesApi.md#create_fiscal_responsibility) | **POST** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities | Create a fiscal responsibility
[**delete_fiscal_responsibility**](FiscalResponsibilitiesApi.md#delete_fiscal_responsibility) | **DELETE** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities/{fiscalResponsibilityId} | Delete a fiscal responsibility
[**get_fiscal_responsibilities**](FiscalResponsibilitiesApi.md#get_fiscal_responsibilities) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{authorityId}/FiscalResponsibilities | Get fiscal responsibilities for an authority
[**get_fiscal_responsibilities_count**](FiscalResponsibilitiesApi.md#get_fiscal_responsibilities_count) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/Count | Get fiscal responsibilities count
[**get_fiscal_responsibility**](FiscalResponsibilitiesApi.md#get_fiscal_responsibility) | **GET** /api/v2/AccountingService/Fiscals/Authorities/{fiscalAuthorityId}/FiscalResponsibilities/{fiscalResponsibilityId} | Get fiscal responsibility by ID
[**update_fiscal_responsibility**](FiscalResponsibilitiesApi.md#update_fiscal_responsibility) | **PUT** /api/v2/AccountingService/Fiscals/Authorities/FiscalResponsibilities/{fiscalResponsibilityId} | Update a fiscal responsibility



## create_fiscal_responsibility

> models::EmptyEnvelope create_fiscal_responsibility(tenant_id, api_version, x_api_version, fiscal_responsibility_create_dto)
Create a fiscal responsibility

Creates a new fiscal responsibility for a fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_responsibility_create_dto** | Option<[**FiscalResponsibilityCreateDto**](FiscalResponsibilityCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_fiscal_responsibility

> models::EmptyEnvelope delete_fiscal_responsibility(tenant_id, fiscal_responsibility_id, api_version, x_api_version)
Delete a fiscal responsibility

Deletes a fiscal responsibility identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_responsibilities

> models::FiscalResponsibilityDtoListEnvelope get_fiscal_responsibilities(fiscal_authority_id, authority_id, api_version, x_api_version)
Get fiscal responsibilities for an authority

Retrieves all fiscal responsibilities for the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**authority_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalResponsibilityDtoListEnvelope**](FiscalResponsibilityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_fiscal_responsibilities_count

> models::Int32Envelope get_fiscal_responsibilities_count(fiscal_authority_id, api_version, x_api_version)
Get fiscal responsibilities count

Returns the total count of fiscal responsibilities for the specified fiscal authority.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
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


## get_fiscal_responsibility

> models::FiscalResponsibilityDtoEnvelope get_fiscal_responsibility(tenant_id, fiscal_authority_id, fiscal_responsibility_id, api_version, x_api_version)
Get fiscal responsibility by ID

Retrieves a specific fiscal responsibility by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_authority_id** | **uuid::Uuid** |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FiscalResponsibilityDtoEnvelope**](FiscalResponsibilityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_fiscal_responsibility

> models::EmptyEnvelope update_fiscal_responsibility(tenant_id, fiscal_responsibility_id, api_version, x_api_version, fiscal_responsibility_update_dto)
Update a fiscal responsibility

Updates an existing fiscal responsibility identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | [**serde_json::Value**](.md) |  | [required] |
**fiscal_responsibility_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**fiscal_responsibility_update_dto** | Option<[**FiscalResponsibilityUpdateDto**](FiscalResponsibilityUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

