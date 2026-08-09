# PostingExecutionDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> |  | [optional]
**timestamp** | Option<**String**> |  | [optional]
**tenant_id** | Option<**String**> |  | [optional]
**enrollment_id** | Option<**String**> |  | [optional]
**posting_intent_id** | Option<**String**> |  | [optional]
**posting_idempotency_key** | Option<**String**> |  | [optional]
**intent_type** | Option<**String**> |  | [optional]
**posting_operation** | Option<**String**> |  | [optional]
**source_document_type** | Option<**String**> |  | [optional]
**source_document_id** | Option<**String**> |  | [optional]
**status** | Option<**String**> |  | [optional]
**failure_kind** | Option<**String**> |  | [optional]
**failure_code** | Option<**String**> |  | [optional]
**retryable** | Option<**bool**> |  | [optional]
**correlation_id** | Option<**String**> |  | [optional]
**causation_id** | Option<**String**> |  | [optional]
**received_at_utc** | Option<**String**> |  | [optional]
**processing_started_at_utc** | Option<**String**> |  | [optional]
**completed_at_utc** | Option<**String**> |  | [optional]
**book_results** | Option<[**Vec<models::PostingBookResultDto>**](PostingBookResultDto.md)> |  | [optional]
**failure_class** | Option<**String**> |  | [optional][readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


