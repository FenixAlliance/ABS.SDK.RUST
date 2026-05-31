# \UploadsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**save_file_async**](UploadsApi.md#save_file_async) | **POST** /api/v2/StorageService/Uploads | Upload a file



## save_file_async

> models::EmptyEnvelope save_file_async(tenant_id, api_version, x_api_version, notes, title, author, is_folder, file_name, r#abstract, key_words, valid_response, parent_file_upload_id, file_path, app_file_period_content, app_file_period_sha256, app_file_period_created_at_utc, app_file_period_user_id_period_value, app_file_period_tenant_id_period_value, app_file_period_enrollment_id_period_value, app_file_period_source, app_file_period_length, app_file_period_name, app_file_period_file_name, app_file_period_last_modified, app_file_period_size, app_file_period_content_type, app_file_period_content_disposition, app_file_period_headers, id, timestamp)
Upload a file

Uploads a file to tenant or user storage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**notes** | Option<**String**> |  |  |
**title** | Option<**String**> |  |  |
**author** | Option<**String**> |  |  |
**is_folder** | Option<**bool**> |  |  |
**file_name** | Option<**String**> |  |  |
**r#abstract** | Option<**String**> |  |  |
**key_words** | Option<**String**> |  |  |
**valid_response** | Option<**bool**> |  |  |
**parent_file_upload_id** | Option<**String**> |  |  |
**file_path** | Option<**String**> |  |  |
**app_file_period_content** | Option<**String**> |  |  |
**app_file_period_sha256** | Option<**String**> |  |  |
**app_file_period_created_at_utc** | Option<**String**> |  |  |
**app_file_period_user_id_period_value** | Option<**uuid::Uuid**> |  |  |
**app_file_period_tenant_id_period_value** | Option<**uuid::Uuid**> |  |  |
**app_file_period_enrollment_id_period_value** | Option<**uuid::Uuid**> |  |  |
**app_file_period_source** | Option<**String**> |  |  |
**app_file_period_length** | Option<**i64**> |  |  |
**app_file_period_name** | Option<**String**> |  |  |
**app_file_period_file_name** | Option<**String**> |  |  |
**app_file_period_last_modified** | Option<**String**> |  |  |
**app_file_period_size** | Option<**i64**> |  |  |
**app_file_period_content_type** | Option<**String**> |  |  |
**app_file_period_content_disposition** | Option<**String**> |  |  |
**app_file_period_headers** | Option<[**std::collections::HashMap<String, String>**](std::collections::HashMap.md)> |  |  |
**id** | Option<**uuid::Uuid**> |  |  |
**timestamp** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

