# \SigningParticipantsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_signing_participant_by_id_async**](SigningParticipantsApi.md#get_signing_participant_by_id_async) | **GET** /api/v2/TrustService/SigningParticipants/{id} | Get signing participant by ID
[**get_signing_participants_async**](SigningParticipantsApi.md#get_signing_participants_async) | **GET** /api/v2/TrustService/SigningParticipants | Get all signing participants
[**get_signing_participants_count_async**](SigningParticipantsApi.md#get_signing_participants_count_async) | **GET** /api/v2/TrustService/SigningParticipants/Count | Get signing participants count
[**mark_viewed_async**](SigningParticipantsApi.md#mark_viewed_async) | **POST** /api/v2/TrustService/SigningParticipants/{id}/viewed | Mark a participant as having viewed the request
[**record_outcome_async**](SigningParticipantsApi.md#record_outcome_async) | **POST** /api/v2/TrustService/SigningParticipants/{id}/outcome | Record a manual/external participant outcome



## get_signing_participant_by_id_async

> models::SigningParticipantDto get_signing_participant_by_id_async(tenant_id, id, api_version, x_api_version)
Get signing participant by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningParticipantDto**](SigningParticipantDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_participants_async

> models::SigningParticipantDtoListEnvelope get_signing_participants_async(tenant_id, api_version, x_api_version)
Get all signing participants

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_signing_participants_count_async

> models::Int32Envelope get_signing_participants_count_async(tenant_id, api_version, x_api_version)
Get signing participants count

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


## mark_viewed_async

> mark_viewed_async(tenant_id, id, api_version, x_api_version)
Mark a participant as having viewed the request

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


## record_outcome_async

> record_outcome_async(tenant_id, id, api_version, x_api_version, record_signing_participant_outcome_dto)
Record a manual/external participant outcome

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**record_signing_participant_outcome_dto** | Option<[**RecordSigningParticipantOutcomeDto**](RecordSigningParticipantOutcomeDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

