# \SigningRequestsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_participant_async**](SigningRequestsApi.md#add_participant_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/participants | Add a participant to a signing request
[**create_from_document_async**](SigningRequestsApi.md#create_from_document_async) | **POST** /api/v2/TrustService/SigningRequests/from-document/{signedDocumentId} | Create a signing request from a frozen document
[**execute_provider_async**](SigningRequestsApi.md#execute_provider_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/execute-provider | Run a signing provider to produce + finalize the signed artifact
[**expire_async**](SigningRequestsApi.md#expire_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/expire | Expire a signing request
[**finalize_async**](SigningRequestsApi.md#finalize_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/finalize | Finalize a completed request into a signed artifact
[**get_signing_request_by_id_async**](SigningRequestsApi.md#get_signing_request_by_id_async) | **GET** /api/v2/TrustService/SigningRequests/{id} | Get signing request by ID
[**get_signing_request_participants_async**](SigningRequestsApi.md#get_signing_request_participants_async) | **GET** /api/v2/TrustService/SigningRequests/{id}/Participants | Get participants of a signing request
[**get_signing_requests_async**](SigningRequestsApi.md#get_signing_requests_async) | **GET** /api/v2/TrustService/SigningRequests | Get all signing requests
[**get_signing_requests_count_async**](SigningRequestsApi.md#get_signing_requests_count_async) | **GET** /api/v2/TrustService/SigningRequests/Count | Get signing requests count
[**prepare_and_create_async**](SigningRequestsApi.md#prepare_and_create_async) | **POST** /api/v2/TrustService/SigningRequests/prepare-and-create | Create, store, freeze a document and open a signing request in one call
[**send_async**](SigningRequestsApi.md#send_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/send | Send a signing request
[**void_async**](SigningRequestsApi.md#void_async) | **POST** /api/v2/TrustService/SigningRequests/{id}/void | Void a signing request



## add_participant_async

> models::SigningParticipantDto add_participant_async(tenant_id, id, api_version, x_api_version, create_signing_participant_dto)
Add a participant to a signing request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**create_signing_participant_dto** | Option<[**CreateSigningParticipantDto**](CreateSigningParticipantDto.md)> |  |  |

### Return type

[**models::SigningParticipantDto**](SigningParticipantDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_from_document_async

> models::SigningRequestDto create_from_document_async(tenant_id, signed_document_id, api_version, x_api_version, create_signing_request_dto)
Create a signing request from a frozen document

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**signed_document_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**create_signing_request_dto** | Option<[**CreateSigningRequestDto**](CreateSigningRequestDto.md)> |  |  |

### Return type

[**models::SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## execute_provider_async

> execute_provider_async(tenant_id, id, api_version, x_api_version, execute_signing_request_dto)
Run a signing provider to produce + finalize the signed artifact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**execute_signing_request_dto** | Option<[**ExecuteSigningRequestDto**](ExecuteSigningRequestDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## expire_async

> expire_async(tenant_id, id, api_version, x_api_version)
Expire a signing request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
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


## finalize_async

> finalize_async(tenant_id, id, api_version, x_api_version, finalize_signing_request_dto)
Finalize a completed request into a signed artifact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**finalize_signing_request_dto** | Option<[**FinalizeSigningRequestDto**](FinalizeSigningRequestDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_request_by_id_async

> models::SigningRequestDto get_signing_request_by_id_async(tenant_id, id, api_version, x_api_version)
Get signing request by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_request_participants_async

> models::SigningParticipantDtoListEnvelope get_signing_request_participants_async(tenant_id, id, api_version, x_api_version)
Get participants of a signing request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningParticipantDtoListEnvelope**](SigningParticipantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_requests_async

> models::SigningRequestDtoListEnvelope get_signing_requests_async(tenant_id, api_version, x_api_version)
Get all signing requests

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningRequestDtoListEnvelope**](SigningRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_requests_count_async

> models::Int32Envelope get_signing_requests_count_async(tenant_id, api_version, x_api_version)
Get signing requests count

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


## prepare_and_create_async

> models::SigningRequestDto prepare_and_create_async(tenant_id, api_version, x_api_version, file, title, contact_id, routing_mode, expires_at_utc, message, correlation_id, external_reference, signers)
Create, store, freeze a document and open a signing request in one call

Server-owned flow (T-UX4): creates a SignedDocument from the uploaded source, stores it, freezes it, then creates a signing request over the frozen artifact and attaches its signers — all in one unit of work. Evidence truth (status/hashes/ids/tokens) is server-produced; the caller supplies intent only. The server generates the new document id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |
**title** | Option<**String**> |  |  |
**contact_id** | Option<**String**> |  |  |
**routing_mode** | Option<**String**> |  |  |
**expires_at_utc** | Option<**String**> |  |  |
**message** | Option<**String**> |  |  |
**correlation_id** | Option<**String**> |  |  |
**external_reference** | Option<**String**> |  |  |
**signers** | Option<**String**> |  |  |

### Return type

[**models::SigningRequestDto**](SigningRequestDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_async

> send_async(tenant_id, id, api_version, x_api_version)
Send a signing request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
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


## void_async

> void_async(tenant_id, id, api_version, x_api_version, void_signing_request_dto)
Void a signing request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**void_signing_request_dto** | Option<[**VoidSigningRequestDto**](VoidSigningRequestDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

