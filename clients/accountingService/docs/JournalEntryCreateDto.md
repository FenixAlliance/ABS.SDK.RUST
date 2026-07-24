# JournalEntryCreateDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**timestamp** | Option<**String**> |  | [optional]
**journal_id** | **String** |  | 
**fiscal_period_id** | **String** |  | 
**transaction_currency_id** | **String** |  | 
**description** | **String** |  | 
**source_document_type** | Option<**String**> |  | [optional]
**source_document_id** | Option<**String**> |  | [optional]
**idempotency_key** | Option<**String**> |  | [optional]
**is_opening_balance** | Option<**bool**> |  | [optional]
**accounting_entries** | Option<[**Vec<models::AccountingEntryCreateDto>**](AccountingEntryCreateDto.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


