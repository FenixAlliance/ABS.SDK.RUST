# \BlobsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_blob_async**](BlobsApi.md#get_blob_async) | **GET** /api/v2/StorageService/Blobs/Single | 
[**get_blobs_async**](BlobsApi.md#get_blobs_async) | **GET** /api/v2/StorageService/Blobs | 



## get_blob_async

> models::BlobEnvelope get_blob_async(tenant_id, file_path, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**file_path** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlobEnvelope**](BlobEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blobs_async

> models::BlobEnvelope get_blobs_async(tenant_id, folder_path, browse_filter, file_prefix, recurse, max_results, include_attributes, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**folder_path** | Option<**String**> |  |  |
**browse_filter** | Option<**String**> |  |  |
**file_prefix** | Option<**String**> |  |  |
**recurse** | Option<**bool**> |  |  |
**max_results** | Option<**i32**> |  |  |
**include_attributes** | Option<**bool**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlobEnvelope**](BlobEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

