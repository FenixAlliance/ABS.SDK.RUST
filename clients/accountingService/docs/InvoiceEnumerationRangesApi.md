# \InvoiceEnumerationRangesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#create_invoice_enumeration_range_async) | **POST** /api/v2/AccountingService/InvoiceEnumerationRanges | Create a new invoice enumeration range
[**delete_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#delete_invoice_enumeration_range_async) | **DELETE** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Delete an invoice enumeration range
[**get_invoice_enumeration_range_details_async**](InvoiceEnumerationRangesApi.md#get_invoice_enumeration_range_details_async) | **GET** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Get invoice enumeration range by ID
[**get_invoice_enumeration_ranges_async**](InvoiceEnumerationRangesApi.md#get_invoice_enumeration_ranges_async) | **GET** /api/v2/AccountingService/InvoiceEnumerationRanges | Get all invoice enumeration ranges
[**update_invoice_enumeration_range_async**](InvoiceEnumerationRangesApi.md#update_invoice_enumeration_range_async) | **PUT** /api/v2/AccountingService/InvoiceEnumerationRanges/{rangeId} | Update an invoice enumeration range



## create_invoice_enumeration_range_async

> models::EmptyEnvelope create_invoice_enumeration_range_async(tenant_id, api_version, x_api_version, invoice_enumeration_range_create_dto)
Create a new invoice enumeration range

Creates a new invoice enumeration range for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**invoice_enumeration_range_create_dto** | Option<[**InvoiceEnumerationRangeCreateDto**](InvoiceEnumerationRangeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice_enumeration_range_async

> models::EmptyEnvelope delete_invoice_enumeration_range_async(tenant_id, range_id, api_version, x_api_version)
Delete an invoice enumeration range

Deletes an invoice enumeration range by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**range_id** | **uuid::Uuid** |  | [required] |
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


## get_invoice_enumeration_range_details_async

> models::InvoiceEnumerationRangeDtoEnvelope get_invoice_enumeration_range_details_async(tenant_id, range_id, api_version, x_api_version)
Get invoice enumeration range by ID

Retrieves the details of a specific invoice enumeration range.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**range_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InvoiceEnumerationRangeDtoEnvelope**](InvoiceEnumerationRangeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_enumeration_ranges_async

> models::InvoiceEnumerationRangeDtoListEnvelope get_invoice_enumeration_ranges_async(tenant_id, api_version, x_api_version)
Get all invoice enumeration ranges

Retrieves all invoice enumeration ranges for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InvoiceEnumerationRangeDtoListEnvelope**](InvoiceEnumerationRangeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice_enumeration_range_async

> models::EmptyEnvelope update_invoice_enumeration_range_async(tenant_id, range_id, api_version, x_api_version, invoice_enumeration_range_update_dto)
Update an invoice enumeration range

Updates an existing invoice enumeration range with the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**range_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**invoice_enumeration_range_update_dto** | Option<[**InvoiceEnumerationRangeUpdateDto**](InvoiceEnumerationRangeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

