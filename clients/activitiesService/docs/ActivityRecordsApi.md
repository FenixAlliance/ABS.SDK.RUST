# \ActivityRecordsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_activity_records_count_async**](ActivityRecordsApi.md#get_activity_records_count_async) | **GET** /api/v2/ActivitiesService/ActivityRecords/Count | Count activity records



## get_activity_records_count_async

> models::Int32Envelope get_activity_records_count_async(tenant_id, api_version, x_api_version)
Count activity records

Returns the tenant-wide count of activity records across all feeds owned by the tenant.

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

