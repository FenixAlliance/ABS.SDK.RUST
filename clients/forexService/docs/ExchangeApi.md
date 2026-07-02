# \ExchangeApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**exchange_amount_async**](ExchangeApi.md#exchange_amount_async) | **GET** /api/v2/ForexService/Exchange/Latest | Exchange currency at latest rates
[**exchange_amount_historical_async**](ExchangeApi.md#exchange_amount_historical_async) | **GET** /api/v2/ForexService/Exchange/History | Exchange currency at historical rates



## exchange_amount_async

> models::MoneyEnvelope exchange_amount_async(amount, source_currency_id, target_currency_id)
Exchange currency at latest rates

Exchange an amount of money from one currency to another using the latest available exchange rates.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**amount** | **f64** |  | [required] |
**source_currency_id** | **String** |  | [required] |
**target_currency_id** | **String** |  | [required] |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## exchange_amount_historical_async

> models::MoneyEnvelope exchange_amount_historical_async(amount, source_currency_id, target_currency_id, date)
Exchange currency at historical rates

Exchange an amount of money from one currency to another using exchange rates from a specific historical date.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**amount** | **f64** |  | [required] |
**source_currency_id** | **String** |  | [required] |
**target_currency_id** | **String** |  | [required] |
**date** | **String** |  | [required] |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

