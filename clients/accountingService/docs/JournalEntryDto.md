# JournalEntryDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> |  | [optional]
**tenant_id** | Option<**String**> |  | [optional]
**enrollment_id** | Option<**String**> |  | [optional]
**journal_id** | Option<**String**> |  | [optional]
**journal_name** | Option<**String**> |  | [optional]
**journal_code** | Option<**String**> |  | [optional]
**fiscal_period_id** | Option<**String**> |  | [optional]
**financial_book_id** | Option<**String**> |  | [optional]
**description** | Option<**String**> |  | [optional]
**entry_type** | Option<**String**> |  | [optional]
**status** | Option<**String**> |  | [optional]
**posting_date** | Option<**String**> |  | [optional]
**is_opening_balance** | Option<**bool**> |  | [optional]
**transaction_currency_id** | Option<**String**> |  | [optional]
**source_document_type** | Option<**String**> |  | [optional]
**source_document_id** | Option<**String**> |  | [optional]
**idempotency_key** | Option<**String**> |  | [optional]
**reversal_of_journal_entry_id** | Option<**String**> |  | [optional]
**posted_by** | Option<**String**> |  | [optional]
**forex_rate** | Option<**f64**> |  | [optional]
**forex_rates_snapshot** | Option<**String**> |  | [optional]
**timestamp** | Option<**String**> |  | [optional]
**debit_in_usd** | Option<**f64**> |  | [optional]
**credit_in_usd** | Option<**f64**> |  | [optional]
**accounting_entries** | Option<[**Vec<models::AccountingEntryDto>**](AccountingEntryDto.md)> |  | [optional]
**total_debit** | Option<**f64**> |  | [optional][readonly]
**total_credit** | Option<**f64**> |  | [optional][readonly]
**total_debit_amount** | Option<[**models::Money**](Money.md)> |  | [optional]
**total_credit_amount** | Option<[**models::Money**](Money.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


