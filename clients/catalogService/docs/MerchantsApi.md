# \MerchantsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_merchant_by_id**](MerchantsApi.md#get_merchant_by_id) | **GET** /api/v2/CatalogService/Merchants/{merchantId} | Get merchant by ID
[**get_merchants**](MerchantsApi.md#get_merchants) | **GET** /api/v2/CatalogService/Merchants | Get all merchants
[**get_merchants_count**](MerchantsApi.md#get_merchants_count) | **GET** /api/v2/CatalogService/Merchants/Count | Count merchants



## get_merchant_by_id

> models::MerchantDtoEnvelope get_merchant_by_id(merchant_id, api_version, x_api_version)
Get merchant by ID

Retrieves a merchant by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**merchant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MerchantDtoEnvelope**](MerchantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_merchants

> models::MerchantDtoListEnvelope get_merchants(api_version, x_api_version)
Get all merchants

Retrieves all merchants, optionally filtered by OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MerchantDtoListEnvelope**](MerchantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_merchants_count

> models::Int32Envelope get_merchants_count(api_version, x_api_version)
Count merchants

Counts the number of merchants, optionally filtered by OData query options.

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

