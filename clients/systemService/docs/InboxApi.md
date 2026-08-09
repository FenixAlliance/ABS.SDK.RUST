# \InboxApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_inbox_message_retry**](InboxApi.md#cancel_inbox_message_retry) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/CancelRetry | Cancel a scheduled inbox retry
[**dead_letter_inbox_message**](InboxApi.md#dead_letter_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/DeadLetter | Manually dead-letter an inbox message
[**expedite_inbox_message**](InboxApi.md#expedite_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Expedite | Expedite a retry-scheduled inbox message
[**get_duplicate_inbox_messages**](InboxApi.md#get_duplicate_inbox_messages) | **GET** /api/v2/SystemService/Inbox/Duplicates | List duplicate-bearing inbox messages
[**get_duplicate_inbox_messages_count**](InboxApi.md#get_duplicate_inbox_messages_count) | **GET** /api/v2/SystemService/Inbox/Duplicates/Count | Count duplicate-bearing inbox messages
[**get_inbox_correlation_chain**](InboxApi.md#get_inbox_correlation_chain) | **GET** /api/v2/SystemService/Inbox/Correlations/{correlationId} | Get an inbox correlation chain
[**get_inbox_health**](InboxApi.md#get_inbox_health) | **GET** /api/v2/SystemService/Inbox/Health | Get durable-inbox processor health
[**get_inbox_message**](InboxApi.md#get_inbox_message) | **GET** /api/v2/SystemService/Inbox/Messages/{id} | Get one inbox message
[**get_inbox_messages**](InboxApi.md#get_inbox_messages) | **GET** /api/v2/SystemService/Inbox/Messages | List inbox messages
[**get_inbox_messages_count**](InboxApi.md#get_inbox_messages_count) | **GET** /api/v2/SystemService/Inbox/Messages/Count | Count inbox messages
[**quarantine_inbox_message**](InboxApi.md#quarantine_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Quarantine | Manually quarantine an inbox message
[**release_inbox_message_lease**](InboxApi.md#release_inbox_message_lease) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/ReleaseLease | Release a stuck inbox lease
[**replay_inbox_message**](InboxApi.md#replay_inbox_message) | **POST** /api/v2/SystemService/Inbox/Messages/{id}/Replay | Replay a terminal inbox message as a new generation



## cancel_inbox_message_retry

> models::EmptyEnvelope cancel_inbox_message_retry(id, api_version, x_api_version, inbox_admin_reason_dto)
Cancel a scheduled inbox retry

Stops a RetryScheduled message from retrying by operator decision, moving it to the terminal Cancelled state (deliberately distinct from DeadLettered so the dead-letter gauge stays honest). The reason is audit-critical. Only a RetryScheduled message can be cancelled. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_admin_reason_dto** | Option<[**InboxAdminReasonDto**](InboxAdminReasonDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## dead_letter_inbox_message

> models::EmptyEnvelope dead_letter_inbox_message(id, api_version, x_api_version, inbox_admin_reason_dto)
Manually dead-letter an inbox message

Manually moves a non-terminal message to the terminal DeadLettered state. The reason is audit-critical. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_admin_reason_dto** | Option<[**InboxAdminReasonDto**](InboxAdminReasonDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## expedite_inbox_message

> models::EmptyEnvelope expedite_inbox_message(id, api_version, x_api_version)
Expedite a retry-scheduled inbox message

Pulls a RetryScheduled message's scheduled instant forward to now so the processor claims it on the next poll, bypassing the remaining backoff. Same row, retry budget untouched. Only a RetryScheduled message can be expedited. Global-administrator only.

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


## get_duplicate_inbox_messages

> models::InboxMessageDtoIReadOnlyListEnvelope get_duplicate_inbox_messages(api_version, x_api_version, inbox_message_dto_collection_query_parameters)
List duplicate-bearing inbox messages

Lists inbox messages that have observed a re-delivery (DeliveryCount > 1) — durable evidence that a source is re-sending, surfaced with DeliveryCount / LastDuplicateReceivedAtUtc. Further OData filtering/paging applies. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_message_dto_collection_query_parameters** | Option<[**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_duplicate_inbox_messages_count

> models::Int32Envelope get_duplicate_inbox_messages_count(api_version, x_api_version, inbox_message_dto_collection_query_parameters)
Count duplicate-bearing inbox messages

Returns the count of duplicate-bearing inbox messages under the same OData shaping as the duplicates list. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_message_dto_collection_query_parameters** | Option<[**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbox_correlation_chain

> models::InboxMessageDtoIReadOnlyListEnvelope get_inbox_correlation_chain(correlation_id, api_version, x_api_version)
Get an inbox correlation chain

Returns every inbox message that shares a correlation id — one logical inbound interaction end-to-end, including its replay generations — oldest-received first. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**correlation_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbox_health

> models::InboxHealthDtoEnvelope get_inbox_health(api_version, x_api_version)
Get durable-inbox processor health

Returns a single snapshot of the durable-inbox processor: whether it is enabled, the per-status counts (received/accepted/processing/retry-scheduled/rejected/quarantined/dead-lettered/cancelled), the age of the oldest accepted message, and the last successful processing instant. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InboxHealthDtoEnvelope**](InboxHealthDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbox_message

> models::InboxMessageDtoEnvelope get_inbox_message(id, api_version, x_api_version)
Get one inbox message

Returns one inbox message's payload-safe detail by id — both lifecycle axes (processing status + independent verification status), the dedup lineage, attempt/generation counters, the recorded failure, and the timestamps. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InboxMessageDtoEnvelope**](InboxMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbox_messages

> models::InboxMessageDtoIReadOnlyListEnvelope get_inbox_messages(api_version, x_api_version, inbox_message_dto_collection_query_parameters)
List inbox messages

Lists durable-inbox messages (payload-safe fields only). Use OData to scope by any projected field — e.g. $filter=Status eq 'Quarantined' for the quarantine review, Status eq 'DeadLettered' for terminal failures, VerificationStatus eq 'Failed' for forged/untrusted callbacks, SourceSystem eq 'stripe', or a ReceivedAtUtc range — and to page/order. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_message_dto_collection_query_parameters** | Option<[**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::InboxMessageDtoIReadOnlyListEnvelope**](InboxMessageDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbox_messages_count

> models::Int32Envelope get_inbox_messages_count(api_version, x_api_version, inbox_message_dto_collection_query_parameters)
Count inbox messages

Returns the count of durable-inbox messages under the same OData shaping as the list read (e.g. $filter=Status eq 'Quarantined'). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_message_dto_collection_query_parameters** | Option<[**InboxMessageDtoCollectionQueryParameters**](InboxMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## quarantine_inbox_message

> models::EmptyEnvelope quarantine_inbox_message(id, api_version, x_api_version, inbox_admin_reason_dto)
Manually quarantine an inbox message

Manually holds a non-terminal message for review in the terminal Quarantined state (e.g. an operator judges it suspicious). The reason is audit-critical. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_admin_reason_dto** | Option<[**InboxAdminReasonDto**](InboxAdminReasonDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## release_inbox_message_lease

> models::EmptyEnvelope release_inbox_message_lease(id, api_version, x_api_version)
Release a stuck inbox lease

Force-releases the lease on a message wedged in Processing (a crashed/hung processor) and returns it to the claimable Accepted state, due now, so the next poll re-drives it. The in-flight attempt is NOT counted — a crash is not a business failure. Only a Processing message can have its lease released. Global-administrator only.

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


## replay_inbox_message

> models::InboxReplayResultDtoEnvelope replay_inbox_message(id, api_version, x_api_version, inbox_admin_reason_dto)
Replay a terminal inbox message as a new generation

Replays a terminal message as a NEW processing generation over its immutable received evidence — the inbox's recovery lever (distinct from the outbox's same-row requeue). A selected replay-generation row is resolved back to its lineage root before replaying, so numbering stays global and collision-free; the new row is claimable at once with a fresh retry budget, and the root's evidence and budget are never mutated. Legal only from a terminal state whose authenticity passed. Returns the new generation's identity. The reason is audit-critical. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**inbox_admin_reason_dto** | Option<[**InboxAdminReasonDto**](InboxAdminReasonDto.md)> |  |  |

### Return type

[**models::InboxReplayResultDtoEnvelope**](InboxReplayResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

