# \CurrenciesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_currencies_async**](CurrenciesApi.md#count_currencies_async) | **GET** /api/v2/GlobeService/Currencies/Count | Count currencies
[**get_currency_by_id_async**](CurrenciesApi.md#get_currency_by_id_async) | **GET** /api/v2/GlobeService/Currencies/{currencyId} | Get currency by ID
[**get_enabled_currencies_async**](CurrenciesApi.md#get_enabled_currencies_async) | **GET** /api/v2/GlobeService/Currencies | Get all currencies



## count_currencies_async

> models::Int32Envelope count_currencies_async(api_version, x_api_version)
Count currencies

Returns the total number of enabled currencies, with optional OData filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_currency_by_id_async

> models::CurrencyDtoEnvelope get_currency_by_id_async(currency_id, api_version, x_api_version)
Get currency by ID

Retrieves a single currency by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**currency_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurrencyDtoEnvelope**](CurrencyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enabled_currencies_async

> models::CurrencyDtoListEnvelope get_enabled_currencies_async(api_version, x_api_version)
Get all currencies

Retrieves the list of all enabled currencies with optional OData pagination and filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurrencyDtoListEnvelope**](CurrencyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

