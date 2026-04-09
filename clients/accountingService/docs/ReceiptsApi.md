# \ReceiptsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_receipt_async**](ReceiptsApi.md#create_receipt_async) | **POST** /api/v2/AccountingService/Receipts | Creates a new receipt
[**delete_receipt_async**](ReceiptsApi.md#delete_receipt_async) | **DELETE** /api/v2/AccountingService/Receipts/{receiptId} | Deletes a receipt
[**get_receipt_details_async**](ReceiptsApi.md#get_receipt_details_async) | **GET** /api/v2/AccountingService/Receipts/{receiptId} | Gets details of a receipt
[**get_receipts_async**](ReceiptsApi.md#get_receipts_async) | **GET** /api/v2/AccountingService/Receipts | Retrieves tenant receipts
[**get_receipts_count_async**](ReceiptsApi.md#get_receipts_count_async) | **GET** /api/v2/AccountingService/Receipts/Count | Gets count of tenant receipts
[**update_receipt_async**](ReceiptsApi.md#update_receipt_async) | **PUT** /api/v2/AccountingService/Receipts/{receiptId} | Updates a receipt



## create_receipt_async

> models::EmptyEnvelope create_receipt_async(tenant_id, receipt_create_dto)
Creates a new receipt

Adds a new receipt record under the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**receipt_create_dto** | [**ReceiptCreateDto**](ReceiptCreateDto.md) |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_receipt_async

> models::EmptyEnvelope delete_receipt_async(tenant_id, receipt_id)
Deletes a receipt

Removes an existing receipt from the tenant’s records.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**receipt_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_receipt_details_async

> models::ReceiptDtoEnvelope get_receipt_details_async(tenant_id, receipt_id)
Gets details of a receipt

Retrieves a specific receipt by its ID for the given tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**receipt_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ReceiptDtoEnvelope**](ReceiptDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_receipts_async

> models::ReceiptDtoIReadOnlyListEnvelope get_receipts_async(tenant_id)
Retrieves tenant receipts

Fetches all receipts for a given tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ReceiptDtoIReadOnlyListEnvelope**](ReceiptDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_receipts_count_async

> models::Int32Envelope get_receipts_count_async(tenant_id)
Gets count of tenant receipts

Returns total number of receipts for the tenant with OData filter support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_receipt_async

> models::EmptyEnvelope update_receipt_async(tenant_id, receipt_id, receipt_update_dto)
Updates a receipt

Modifies the data of an existing receipt for the given tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**receipt_id** | **uuid::Uuid** |  | [required] |
**receipt_update_dto** | [**ReceiptUpdateDto**](ReceiptUpdateDto.md) |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

