# \FilesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_file_async**](FilesApi.md#create_file_async) | **POST** /api/v2/StorageService/Files | 
[**delete_file_async**](FilesApi.md#delete_file_async) | **DELETE** /api/v2/StorageService/Files/{fileId} | 
[**download_file_async**](FilesApi.md#download_file_async) | **GET** /api/v2/StorageService/Files/{fileId}/Raw | 
[**get_file_async**](FilesApi.md#get_file_async) | **GET** /api/v2/StorageService/Files/{fileId} | 
[**get_files_async**](FilesApi.md#get_files_async) | **GET** /api/v2/StorageService/Files | 
[**update_file_async**](FilesApi.md#update_file_async) | **PUT** /api/v2/StorageService/Files/{fileId} | 



## create_file_async

> models::EmptyEnvelope create_file_async(tenant_id, api_version, x_api_version, id, timestamp, notes, title, author, is_folder, file_name, r#abstract, key_words, valid_response, parent_file_upload_id, file_path, file)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**id** | Option<**uuid::Uuid**> |  |  |
**timestamp** | Option<**String**> |  |  |
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
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_file_async

> models::FileUploadDtoEnvelope delete_file_async(file_id, tenant_id, api_version, x_api_version)


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


## update_file_async

> models::FileUploadDtoEnvelope update_file_async(file_id, tenant_id, api_version, x_api_version, notes, metadata, title, author, is_folder, file_name, r#abstract, key_words, valid_response, parent_file_upload_id, file_path, file)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
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
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::FileUploadDtoEnvelope**](FileUploadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, image/png

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

