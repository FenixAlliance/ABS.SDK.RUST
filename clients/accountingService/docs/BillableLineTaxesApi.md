# \BillableLineTaxesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_billable_line_tax**](BillableLineTaxesApi.md#create_billable_line_tax) | **POST** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes | Create a new tax for a billable line.
[**delete_billable_line_tax**](BillableLineTaxesApi.md#delete_billable_line_tax) | **DELETE** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/{taxId} | Delete a tax from a billable line.
[**get_billable_line_taxes**](BillableLineTaxesApi.md#get_billable_line_taxes) | **GET** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes | Get taxes for a billable line.
[**get_billable_line_taxes_count**](BillableLineTaxesApi.md#get_billable_line_taxes_count) | **GET** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/Count | Get the count of taxes for a billable line.
[**update_billable_line_tax**](BillableLineTaxesApi.md#update_billable_line_tax) | **PUT** /api/v2/AccountingService/BillableLines/{billableLineId}/Taxes/{taxId} | Update a tax for a billable line.



## create_billable_line_tax

> models::EmptyEnvelope create_billable_line_tax(tenant_id, billable_line_id, api_version, x_api_version, applied_item_tax_record_create_dto)
Create a new tax for a billable line.

Creates a new tax entry for the specified billable line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billable_line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**applied_item_tax_record_create_dto** | Option<[**AppliedItemTaxRecordCreateDto**](AppliedItemTaxRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_billable_line_tax

> models::EmptyEnvelope delete_billable_line_tax(tenant_id, billable_line_id, tax_id, api_version, x_api_version)
Delete a tax from a billable line.

Deletes the specified tax entry from the billable line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billable_line_id** | **uuid::Uuid** |  | [required] |
**tax_id** | **uuid::Uuid** |  | [required] |
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


## get_billable_line_taxes

> models::AppliedItemTaxRecordDtoIReadOnlyListEnvelope get_billable_line_taxes(tenant_id, billable_line_id, api_version, x_api_version)
Get taxes for a billable line.

Retrieves the taxes applied to the specified billable line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billable_line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppliedItemTaxRecordDtoIReadOnlyListEnvelope**](AppliedItemTaxRecordDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_billable_line_taxes_count

> models::Int32Envelope get_billable_line_taxes_count(tenant_id, billable_line_id, api_version, x_api_version)
Get the count of taxes for a billable line.

Retrieves the total count of taxes applied to the specified billable line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billable_line_id** | **uuid::Uuid** |  | [required] |
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


## update_billable_line_tax

> models::EmptyEnvelope update_billable_line_tax(tenant_id, billable_line_id, tax_id, api_version, x_api_version, applied_item_tax_record_update_dto)
Update a tax for a billable line.

Updates the specified tax entry for the billable line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billable_line_id** | **uuid::Uuid** |  | [required] |
**tax_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**applied_item_tax_record_update_dto** | Option<[**AppliedItemTaxRecordUpdateDto**](AppliedItemTaxRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

