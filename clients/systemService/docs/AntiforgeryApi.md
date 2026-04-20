# \AntiforgeryApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_and_store_tokens**](AntiforgeryApi.md#get_and_store_tokens) | **GET** /api/v2/SystemService/Antiforgery/GetAndStoreTokens | Get and store antiforgery tokens
[**is_request_valid_async**](AntiforgeryApi.md#is_request_valid_async) | **GET** /api/v2/SystemService/Antiforgery/IsRequestValid | Validate antiforgery request



## get_and_store_tokens

> get_and_store_tokens(api_version, x_api_version)
Get and store antiforgery tokens

Generates antiforgery tokens and stores them in the current HTTP context.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## is_request_valid_async

> is_request_valid_async(api_version, x_api_version)
Validate antiforgery request

Validates whether the current HTTP request contains a valid antiforgery token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

