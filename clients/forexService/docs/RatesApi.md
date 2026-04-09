# \RatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_historical_currency_rate_async**](RatesApi.md#get_historical_currency_rate_async) | **GET** /api/v2/ForexService/Rates/History/{currencyId} | Get historical rate for a currency
[**get_historical_currency_rates_async**](RatesApi.md#get_historical_currency_rates_async) | **GET** /api/v2/ForexService/Rates/History | Get historical currency rates
[**get_latest_currency_rate_async**](RatesApi.md#get_latest_currency_rate_async) | **GET** /api/v2/ForexService/Rates/Latest/{currencyId} | Get latest rate for a currency
[**get_latest_currency_rates_model_async**](RatesApi.md#get_latest_currency_rates_model_async) | **GET** /api/v2/ForexService/Rates/Latest | Get latest currency rates



## get_historical_currency_rate_async

> models::ExchangeRateEnvelope get_historical_currency_rate_async(currency_id, date, api_version, x_api_version)
Get historical rate for a currency

Retrieves the exchange rate for a specific currency as of a specific historical date.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**currency_id** | **String** |  | [required] |
**date** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_historical_currency_rates_async

> models::ForexRatesDtoEnvelope get_historical_currency_rates_async(date, api_version, x_api_version)
Get historical currency rates

Retrieves exchange rates for all supported currencies as of a specific historical date.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**date** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ForexRatesDtoEnvelope**](ForexRatesDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_latest_currency_rate_async

> models::ExchangeRateEnvelope get_latest_currency_rate_async(currency_id, api_version, x_api_version)
Get latest rate for a currency

Retrieves the latest exchange rate for a specific currency by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**currency_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_latest_currency_rates_model_async

> models::ForexRatesDtoEnvelope get_latest_currency_rates_model_async(api_version, x_api_version)
Get latest currency rates

Retrieves the latest exchange rates for all supported currencies.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ForexRatesDtoEnvelope**](ForexRatesDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

