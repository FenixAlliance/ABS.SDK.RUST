# \ExchangeVApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**exchange_amount_historical_v3_async**](ExchangeVApi.md#exchange_amount_historical_v3_async) | **GET** /api/v3/ForexService/Exchange/History | Exchange currency at historical rates (v3)
[**exchange_amount_v3_async**](ExchangeVApi.md#exchange_amount_v3_async) | **GET** /api/v3/ForexService/Exchange/Latest | Exchange currency at latest rates (v3)



## exchange_amount_historical_v3_async

> models::ExchangeRateEnvelope exchange_amount_historical_v3_async(amount, source_currency_id, target_currency_id, date)
Exchange currency at historical rates (v3)

Exchange an amount of money from one currency to another using exchange rates from a specific historical date. Returns the full ExchangeRate details.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**amount** | **f64** |  | [required] |
**source_currency_id** | **String** |  | [required] |
**target_currency_id** | **String** |  | [required] |
**date** | **String** |  | [required] |

### Return type

[**models::ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## exchange_amount_v3_async

> models::ExchangeRateEnvelope exchange_amount_v3_async(amount, source_currency_id, target_currency_id)
Exchange currency at latest rates (v3)

Exchange an amount of money from one currency to another using the latest available exchange rates. Returns the full ExchangeRate details.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**amount** | **f64** |  | [required] |
**source_currency_id** | **String** |  | [required] |
**target_currency_id** | **String** |  | [required] |

### Return type

[**models::ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

