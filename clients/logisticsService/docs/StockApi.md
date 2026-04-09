# \StockApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_contacts_async**](StockApi.md#get_contacts_async) | **GET** /api/v2/LogisticsService/Stock | Get all stock-related contacts



## get_contacts_async

> models::ContactDtoListEnvelope get_contacts_async(tenant_id, api_version, x_api_version)
Get all stock-related contacts

Retrieves all business-owned contacts related to stock and logistics for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

