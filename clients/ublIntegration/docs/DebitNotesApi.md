# \DebitNotesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v2_ubl_service_debit_notes_invoice_id_get**](DebitNotesApi.md#api_v2_ubl_service_debit_notes_invoice_id_get) | **GET** /api/v2/UblService/DebitNotes/{invoiceId} | 



## api_v2_ubl_service_debit_notes_invoice_id_get

> api_v2_ubl_service_debit_notes_invoice_id_get(tenant_id, invoice_id, profile, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**profile** | Option<**String**> |  |  |[default to Generic]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

