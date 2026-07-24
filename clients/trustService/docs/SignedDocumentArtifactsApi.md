# \SignedDocumentArtifactsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**freeze_async**](SignedDocumentArtifactsApi.md#freeze_async) | **POST** /api/v2/TrustService/SignedDocumentArtifacts/{signedDocumentId}/freeze | Freeze the source for signature
[**get_reference_async**](SignedDocumentArtifactsApi.md#get_reference_async) | **GET** /api/v2/TrustService/SignedDocumentArtifacts/reference/{fileUploadId} | Get an artifact reference
[**set_primary_authoring_file_async**](SignedDocumentArtifactsApi.md#set_primary_authoring_file_async) | **PUT** /api/v2/TrustService/SignedDocumentArtifacts/{signedDocumentId}/primary-file/{fileUploadId} | Set the primary authoring file
[**verify_async**](SignedDocumentArtifactsApi.md#verify_async) | **GET** /api/v2/TrustService/SignedDocumentArtifacts/reference/{fileUploadId}/verify | Verify an artifact hash



## freeze_async

> models::TrustArtifactReferenceDtoEnvelope freeze_async(tenant_id, signed_document_id, api_version, x_api_version)
Freeze the source for signature

Copies the primary authoring artifact into a new Sealed frozen-source artifact, hashes it, and binds it to the document (LockState = FrozenForSignature).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**signed_document_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrustArtifactReferenceDtoEnvelope**](TrustArtifactReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_reference_async

> models::TrustArtifactReferenceDtoEnvelope get_reference_async(tenant_id, file_upload_id, api_version, x_api_version)
Get an artifact reference

Resolves a stored artifact's reference (FileUpload id + key + hash + media hints).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**file_upload_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrustArtifactReferenceDtoEnvelope**](TrustArtifactReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_primary_authoring_file_async

> set_primary_authoring_file_async(tenant_id, signed_document_id, file_upload_id, api_version, x_api_version)
Set the primary authoring file

Links an existing scan-gated FileUpload as the document's mutable authoring artifact (only while editable).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**signed_document_id** | **String** |  | [required] |
**file_upload_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## verify_async

> models::BooleanEnvelope verify_async(tenant_id, file_upload_id, api_version, x_api_version)
Verify an artifact hash

Re-reads the artifact bytes and verifies them against the recorded SHA-256. Returns true on match.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**file_upload_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

