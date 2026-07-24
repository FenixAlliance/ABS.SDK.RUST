# \RadzenEditorApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**radzen_upload_image**](RadzenEditorApi.md#radzen_upload_image) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/upload/image | Upload an editor image to tenant storage.
[**radzen_upload_image_scoped**](RadzenEditorApi.md#radzen_upload_image_scoped) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/image | Upload an editor image scoped to a record.
[**radzen_upload_single**](RadzenEditorApi.md#radzen_upload_single) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/upload/single | Upload a single editor file to tenant storage.
[**radzen_upload_single_scoped**](RadzenEditorApi.md#radzen_upload_single_scoped) | **POST** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/single | Upload a single editor file scoped to a record.
[**radzen_upload_stream**](RadzenEditorApi.md#radzen_upload_stream) | **PUT** /api/v2/fs/radzen/tenants/{tenantId}/upload/stream | Chunked editor upload (not implemented).
[**radzen_upload_stream_scoped**](RadzenEditorApi.md#radzen_upload_stream_scoped) | **PUT** /api/v2/fs/radzen/tenants/{tenantId}/{recordType}/{recordId}/upload/stream | Chunked editor upload scoped to a record (not implemented).
[**radzen_upload_user_image**](RadzenEditorApi.md#radzen_upload_user_image) | **POST** /api/v2/fs/radzen/users/upload/image | Upload an editor image to user storage.
[**radzen_upload_user_image_scoped**](RadzenEditorApi.md#radzen_upload_user_image_scoped) | **POST** /api/v2/fs/radzen/users/{recordType}/{recordId}/upload/image | Upload a user editor image scoped to a record.



## radzen_upload_image

> radzen_upload_image(tenant_id, visibility, social_profile_id, purpose, api_version, x_api_version, file)
Upload an editor image to tenant storage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**visibility** | Option<**String**> |  |  |
**social_profile_id** | Option<**String**> |  |  |
**purpose** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## radzen_upload_image_scoped

> radzen_upload_image_scoped(tenant_id, record_type, record_id, visibility, social_profile_id, purpose, api_version, x_api_version, file)
Upload an editor image scoped to a record.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**record_type** | **String** |  | [required] |
**record_id** | **String** |  | [required] |
**visibility** | Option<**String**> |  |  |
**social_profile_id** | Option<**String**> |  |  |
**purpose** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## radzen_upload_single

> radzen_upload_single(tenant_id, api_version, x_api_version, file)
Upload a single editor file to tenant storage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## radzen_upload_single_scoped

> radzen_upload_single_scoped(tenant_id, record_type, record_id, api_version, x_api_version, file)
Upload a single editor file scoped to a record.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**record_type** | **String** |  | [required] |
**record_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## radzen_upload_stream

> radzen_upload_stream(tenant_id, api_version, x_api_version)
Chunked editor upload (not implemented).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **String** |  | [required] |
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


## radzen_upload_stream_scoped

> radzen_upload_stream_scoped(tenant_id, record_type, record_id, api_version, x_api_version)
Chunked editor upload scoped to a record (not implemented).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **String** |  | [required] |
**record_type** | **String** |  | [required] |
**record_id** | **String** |  | [required] |
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


## radzen_upload_user_image

> radzen_upload_user_image(visibility, social_profile_id, purpose, api_version, x_api_version, file)
Upload an editor image to user storage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**visibility** | Option<**String**> |  |  |
**social_profile_id** | Option<**String**> |  |  |
**purpose** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## radzen_upload_user_image_scoped

> radzen_upload_user_image_scoped(record_type, record_id, visibility, social_profile_id, purpose, api_version, x_api_version, file)
Upload a user editor image scoped to a record.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_type** | **String** |  | [required] |
**record_id** | **String** |  | [required] |
**visibility** | Option<**String**> |  |  |
**social_profile_id** | Option<**String**> |  |  |
**purpose** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

