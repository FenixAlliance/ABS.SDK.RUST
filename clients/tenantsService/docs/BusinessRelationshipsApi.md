# \BusinessRelationshipsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_business_relationships_count_async**](BusinessRelationshipsApi.md#get_business_relationships_count_async) | **GET** /api/v2/TenantsService/BusinessRelationships/Count | Get business relationships count



## get_business_relationships_count_async

> models::Int32Envelope get_business_relationships_count_async(tenant_id, api_version, x_api_version)
Get business relationships count

Returns the count of child business relationships owned by the specified parent tenant.

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

