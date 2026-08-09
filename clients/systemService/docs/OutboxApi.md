# \OutboxApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_outbox_message**](OutboxApi.md#cancel_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Cancel | Cancel an outbox message
[**dead_letter_outbox_message**](OutboxApi.md#dead_letter_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/DeadLetter | Manually dead-letter an outbox message
[**expedite_outbox_message**](OutboxApi.md#expedite_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Expedite | Expedite a failed (retry-eligible) outbox message
[**get_outbox_correlation_chain**](OutboxApi.md#get_outbox_correlation_chain) | **GET** /api/v2/SystemService/Outbox/Correlations/{correlationId} | Get an outbox correlation chain
[**get_outbox_health**](OutboxApi.md#get_outbox_health) | **GET** /api/v2/SystemService/Outbox/Health | Get durable-outbox relay health
[**get_outbox_message**](OutboxApi.md#get_outbox_message) | **GET** /api/v2/SystemService/Outbox/Messages/{id} | Get one outbox message
[**get_outbox_messages**](OutboxApi.md#get_outbox_messages) | **GET** /api/v2/SystemService/Outbox/Messages | List outbox messages
[**get_outbox_messages_count**](OutboxApi.md#get_outbox_messages_count) | **GET** /api/v2/SystemService/Outbox/Messages/Count | Count outbox messages
[**release_outbox_message_lease**](OutboxApi.md#release_outbox_message_lease) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/ReleaseLease | Release a stuck outbox lease
[**replay_outbox_message**](OutboxApi.md#replay_outbox_message) | **POST** /api/v2/SystemService/Outbox/Messages/{id}/Replay | Replay a dead-lettered or failed outbox message



## cancel_outbox_message

> models::EmptyEnvelope cancel_outbox_message(id, api_version, x_api_version, outbox_admin_reason_dto)
Cancel an outbox message

Stops a Pending or Failed message by operator decision, moving it to the terminal Cancelled state (deliberately distinct from DeadLettered so the dead-letter gauge stays honest). The reason is audit-critical. An in-flight (Processing) or already-terminal message is rejected. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**outbox_admin_reason_dto** | Option<[**OutboxAdminReasonDto**](OutboxAdminReasonDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## dead_letter_outbox_message

> models::EmptyEnvelope dead_letter_outbox_message(id, api_version, x_api_version, outbox_admin_reason_dto)
Manually dead-letter an outbox message

Manually moves a Processing or Failed message to the terminal DeadLettered state. The reason is audit-critical. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**outbox_admin_reason_dto** | Option<[**OutboxAdminReasonDto**](OutboxAdminReasonDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## expedite_outbox_message

> models::EmptyEnvelope expedite_outbox_message(id, api_version, x_api_version)
Expedite a failed (retry-eligible) outbox message

Pulls a Failed message's scheduled instant forward to now so the relay claims it on the next poll, bypassing the remaining backoff. Same row, retry budget untouched (the lighter-touch counterpart to Replay, which also clears the recorded error). Only a Failed message can be expedited. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outbox_correlation_chain

> models::OutboxMessageDtoIReadOnlyListEnvelope get_outbox_correlation_chain(correlation_id, api_version, x_api_version)
Get an outbox correlation chain

Returns every outbox message that shares a correlation id — one logical unit of async work end-to-end (e.g. a command and the events its handler in turn staged) — oldest-created first. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**correlation_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OutboxMessageDtoIReadOnlyListEnvelope**](OutboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outbox_health

> models::OutboxHealthDtoEnvelope get_outbox_health(api_version, x_api_version)
Get durable-outbox relay health

Returns a single snapshot of the durable-outbox relay: whether it is enabled, the per-status counts (pending/processing/failed/dead-lettered), the age of the oldest pending message, and the last successful dispatch instant. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OutboxHealthDtoEnvelope**](OutboxHealthDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outbox_message

> models::OutboxMessageDtoEnvelope get_outbox_message(id, api_version, x_api_version)
Get one outbox message

Returns one outbox message's payload-safe detail by id — its lifecycle status, the two classification axes (kind + message type), the attempt/ceiling budget, the recorded failure, the idempotency + correlation lineage, and the timestamps. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OutboxMessageDtoEnvelope**](OutboxMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outbox_messages

> models::OutboxMessageDtoIReadOnlyListEnvelope get_outbox_messages(api_version, x_api_version, outbox_message_dto_collection_query_parameters)
List outbox messages

Lists durable-outbox messages (payload-safe fields only). Use OData to scope to a state — e.g. $filter=Status eq 'DeadLettered' for the dead-letter set or Status eq 'Failed' for retry-eligible rows — and to page/order. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**outbox_message_dto_collection_query_parameters** | Option<[**OutboxMessageDtoCollectionQueryParameters**](OutboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::OutboxMessageDtoIReadOnlyListEnvelope**](OutboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outbox_messages_count

> models::Int32Envelope get_outbox_messages_count(api_version, x_api_version, outbox_message_dto_collection_query_parameters)
Count outbox messages

Returns the count of durable-outbox messages under the same OData shaping as the list read (e.g. $filter=Status eq 'DeadLettered'). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**outbox_message_dto_collection_query_parameters** | Option<[**OutboxMessageDtoCollectionQueryParameters**](OutboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## release_outbox_message_lease

> models::EmptyEnvelope release_outbox_message_lease(id, api_version, x_api_version)
Release a stuck outbox lease

Force-releases the lease on a message wedged in Processing (a crashed/hung relay) and returns it to the claimable Pending state, due now, so the next poll re-drives it. The in-flight attempt is NOT counted — a crash is not a business failure. The relay auto-reclaims a crashed row once its lease expires; this manual lever forces the release immediately. Only a Processing message can have its lease released. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## replay_outbox_message

> models::EmptyEnvelope replay_outbox_message(id, api_version, x_api_version)
Replay a dead-lettered or failed outbox message

Requeues a DeadLettered or Failed message back to Pending so the relay re-drives it immediately (clearing the lease and recorded error, and bypassing the remaining backoff). The attempt budget is preserved — a replay grants one more pass, not a fresh budget. Replaying a message that is already Pending/Processing or is Succeeded/Cancelled is rejected. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

