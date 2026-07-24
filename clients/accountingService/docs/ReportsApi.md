# \ReportsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_trial_balance_async**](ReportsApi.md#get_trial_balance_async) | **GET** /api/v2/AccountingService/Reports/TrialBalance | Trial balance for a fiscal period



## get_trial_balance_async

> models::TrialBalanceDtoEnvelope get_trial_balance_async(tenant_id, fiscal_period_id, financial_book_id, currency_id, api_version, x_api_version)
Trial balance for a fiscal period

Returns the per-account posted debit/credit totals for the given fiscal period (optionally scoped to a single financial book), plus grand totals and the Σdebits == Σcredits balanced flag. Amounts are normalized to the target currency (default USD) from the stored USD reporting amounts.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**fiscal_period_id** | **uuid::Uuid** |  | [required] |
**financial_book_id** | Option<**uuid::Uuid**> |  |  |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TrialBalanceDtoEnvelope**](TrialBalanceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

