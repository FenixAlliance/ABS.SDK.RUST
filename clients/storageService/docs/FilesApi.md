# \FilesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_file_async**](FilesApi.md#create_file_async) | **POST** /api/v2/StorageService/Files | 
[**delete_file_async**](FilesApi.md#delete_file_async) | **DELETE** /api/v2/StorageService/Files/{fileId} | 
[**download_file_async**](FilesApi.md#download_file_async) | **GET** /api/v2/StorageService/Files/{fileId}/Raw | 
[**get_file_async**](FilesApi.md#get_file_async) | **GET** /api/v2/StorageService/Files/{fileId} | 
[**get_file_thumbnail_async**](FilesApi.md#get_file_thumbnail_async) | **GET** /api/v2/StorageService/Files/{fileId}/Thumbnail | 
[**get_files_async**](FilesApi.md#get_files_async) | **GET** /api/v2/StorageService/Files | 
[**get_files_count_async**](FilesApi.md#get_files_count_async) | **GET** /api/v2/StorageService/Files/Count | 
[**update_file_async**](FilesApi.md#update_file_async) | **PUT** /api/v2/StorageService/Files/{fileId} | 



## create_file_async

> models::EmptyEnvelope create_file_async(tenant_id, api_version, x_api_version, file, notes, title, author, is_folder, file_name, r#abstract, key_words, valid_response, parent_file_upload_id, file_path, public_access_type, purpose, social_profile_id_period_value, app_file_period_content, app_file_period_sha256, app_file_period_created_at_utc, app_file_period_user_id_period_value, app_file_period_tenant_id_period_value, app_file_period_enrollment_id_period_value, app_file_period_source, app_file_period_length, app_file_period_name, app_file_period_file_name, app_file_period_last_modified, app_file_period_size, app_file_period_content_type, app_file_period_content_disposition, app_file_period_headers, id, timestamp)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |
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
**public_access_type** | Option<**String**> |  |  |
**purpose** | Option<**String**> |  |  |
**social_profile_id_period_value** | Option<**uuid::Uuid**> |  |  |
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
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_file_async

> models::EmptyEnvelope delete_file_async(file_id, tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## download_file_async

> std::path::PathBuf download_file_async(file_id, tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_file_async

> models::FileUploadDtoEnvelope get_file_async(file_id, tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FileUploadDtoEnvelope**](FileUploadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_file_thumbnail_async

> std::path::PathBuf get_file_thumbnail_async(file_id, tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_files_async

> models::FileUploadDtoEnvelope get_files_async(tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FileUploadDtoEnvelope**](FileUploadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_files_count_async

> i64 get_files_count_async(tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

**i64**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_file_async

> models::EmptyEnvelope update_file_async(file_id, tenant_id, api_version, x_api_version, file, notes, metadata, title, author, is_folder, file_name, r#abstract, key_words, valid_response, parent_file_upload_id, file_path, app_file_period_content, app_file_period_sha256, app_file_period_created_at_utc, app_file_period_user_id_period_value, app_file_period_tenant_id_period_value, app_file_period_enrollment_id_period_value, app_file_period_source, app_file_period_length, app_file_period_name, app_file_period_file_name, app_file_period_last_modified, app_file_period_size, app_file_period_content_type, app_file_period_content_disposition, app_file_period_headers)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |
**notes** | Option<**String**> |  |  |
**metadata** | Option<**String**> |  |  |
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

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

