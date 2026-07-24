# \SignedDocumentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signed_document_async**](SignedDocumentsApi.md#create_signed_document_async) | **POST** /api/v2/TrustService/SignedDocuments | Create a new signed document
[**delete_signed_document_async**](SignedDocumentsApi.md#delete_signed_document_async) | **DELETE** /api/v2/TrustService/SignedDocuments/{id} | Delete a signed document
[**get_signed_document_by_id_async**](SignedDocumentsApi.md#get_signed_document_by_id_async) | **GET** /api/v2/TrustService/SignedDocuments/{id} | Get signed document by ID
[**get_signed_documents_async**](SignedDocumentsApi.md#get_signed_documents_async) | **GET** /api/v2/TrustService/SignedDocuments | Get all signed documents
[**get_signed_documents_count_async**](SignedDocumentsApi.md#get_signed_documents_count_async) | **GET** /api/v2/TrustService/SignedDocuments/Count | Get signed documents count
[**patch_signed_document_async**](SignedDocumentsApi.md#patch_signed_document_async) | **PATCH** /api/v2/TrustService/SignedDocuments/{id} | Patch a signed document
[**prepare_and_quick_sign_async**](SignedDocumentsApi.md#prepare_and_quick_sign_async) | **POST** /api/v2/TrustService/SignedDocuments/prepare-and-quick-sign | Create, freeze, and quick-sign a document in one call
[**quick_sign_signed_document_async**](SignedDocumentsApi.md#quick_sign_signed_document_async) | **POST** /api/v2/TrustService/SignedDocuments/{id}/quick-sign | Quick-sign a frozen document
[**update_signed_document_async**](SignedDocumentsApi.md#update_signed_document_async) | **PUT** /api/v2/TrustService/SignedDocuments/{id} | Update a signed document
[**verify_signed_document_signature_async**](SignedDocumentsApi.md#verify_signed_document_signature_async) | **GET** /api/v2/TrustService/SignedDocuments/{id}/verify-signature | Verify a signed document's signature



## create_signed_document_async

> create_signed_document_async(tenant_id, api_version, x_api_version, signed_document_create_dto)
Create a new signed document

Creates a new signed document for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signed_document_create_dto** | Option<[**SignedDocumentCreateDto**](SignedDocumentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_signed_document_async

> delete_signed_document_async(tenant_id, id, api_version, x_api_version)
Delete a signed document

Deletes a signed document for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_signed_document_by_id_async

> models::SignedDocumentDto get_signed_document_by_id_async(tenant_id, id, api_version, x_api_version)
Get signed document by ID

Retrieves a specific signed document by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignedDocumentDto**](SignedDocumentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signed_documents_async

> models::SignedDocumentDtoListEnvelope get_signed_documents_async(tenant_id, api_version, x_api_version)
Get all signed documents

Retrieves all signed documents for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignedDocumentDtoListEnvelope**](SignedDocumentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signed_documents_count_async

> models::Int32Envelope get_signed_documents_count_async(tenant_id, api_version, x_api_version)
Get signed documents count

Returns the count of signed documents for the specified tenant.

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


## patch_signed_document_async

> models::EmptyEnvelope patch_signed_document_async(tenant_id, id, api_version, x_api_version, operation)
Patch a signed document

Patch a signed document

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## prepare_and_quick_sign_async

> models::SignedDocumentDto prepare_and_quick_sign_async(tenant_id, api_version, x_api_version, id, file, title, contact_id, signing_certificate_id, signing_profile_id, provider_name)
Create, freeze, and quick-sign a document in one call

Server-side single-signer flow: creates a SignedDocument from the uploaded source, stores it, freezes it, signs it with the chosen certificate + provider, and seals it — all in one unit of work. Returns the sealed document. Evidence truth (signed/status/hashes/artifact ids) is server-produced and cannot be supplied by the caller.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**id** | Option<**uuid::Uuid**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |
**title** | Option<**String**> |  |  |
**contact_id** | Option<**String**> |  |  |
**signing_certificate_id** | Option<**String**> |  |  |
**signing_profile_id** | Option<**String**> |  |  |
**provider_name** | Option<**String**> |  |  |

### Return type

[**models::SignedDocumentDto**](SignedDocumentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## quick_sign_signed_document_async

> quick_sign_signed_document_async(tenant_id, id, api_version, x_api_version, quick_sign_signed_document_dto)
Quick-sign a frozen document

Signs a frozen signed document directly with a chosen certificate + provider (no signing-request workflow) and seals it. Returns the sealed document.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**quick_sign_signed_document_dto** | Option<[**QuickSignSignedDocumentDto**](QuickSignSignedDocumentDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_signed_document_async

> update_signed_document_async(tenant_id, id, api_version, x_api_version, signed_document_update_dto)
Update a signed document

Updates an existing signed document for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signed_document_update_dto** | Option<[**SignedDocumentUpdateDto**](SignedDocumentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## verify_signed_document_signature_async

> models::SignatureVerificationDto verify_signed_document_signature_async(tenant_id, id, api_version, x_api_version)
Verify a signed document's signature

Re-verifies the document's signature against its stored signed artifact (bytes intact + signed by the embedded certificate; certificate trust is a separate concern).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignatureVerificationDto**](SignatureVerificationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

