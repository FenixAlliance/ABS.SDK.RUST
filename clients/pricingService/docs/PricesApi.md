# \PricesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_final_price**](PricesApi.md#get_final_price) | **GET** /api/v2/PricingService/Prices/{itemId}/FinalPrice | Gets the final price for an item
[**get_price**](PricesApi.md#get_price) | **GET** /api/v2/PricingService/Prices/{itemId}/Price | Gets the calculated price for an item
[**get_total_savings_in_usd**](PricesApi.md#get_total_savings_in_usd) | **GET** /api/v2/PricingService/Prices/{itemId}/TotalSavings | Gets total savings for an item
[**get_total_taxes_in_usd**](PricesApi.md#get_total_taxes_in_usd) | **GET** /api/v2/PricingService/Prices/{itemId}/TotalTaxes | Gets total taxes for an item



## get_final_price

> models::MoneyEnvelope get_final_price(item_id, currency_id, api_version, x_api_version)
Gets the final price for an item

Gets the final price for an item after all discounts and taxes in the specified currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price

> models::ItemPriceCalculationEnvelope get_price(item_id, price_list_id, discounts_list_id, quantity, currency_id, api_version, x_api_version)
Gets the calculated price for an item

Calculates the price for an item considering price list, discount list, quantity, and currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | Option<**uuid::Uuid**> |  |  |
**discounts_list_id** | Option<**uuid::Uuid**> |  |  |
**quantity** | Option<**f64**> |  |  |[default to 1]
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPriceCalculationEnvelope**](ItemPriceCalculationEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_total_savings_in_usd

> models::MoneyEnvelope get_total_savings_in_usd(item_id, currency_id, api_version, x_api_version)
Gets total savings for an item

Gets the total savings amount for an item in the specified currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_total_taxes_in_usd

> models::MoneyEnvelope get_total_taxes_in_usd(item_id, currency_id, api_version, x_api_version)
Gets total taxes for an item

Gets the total tax amount for an item in the specified currency.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**currency_id** | Option<**String**> |  |  |[default to USD.USA]
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

