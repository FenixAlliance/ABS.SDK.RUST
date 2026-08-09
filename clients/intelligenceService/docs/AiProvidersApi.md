# \AiProvidersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_ai_providers_async**](AiProvidersApi.md#get_ai_providers_async) | **GET** /api/v2/IntelligenceService/AiProviders | Get the available AI providers



## get_ai_providers_async

> models::AiProviderDtoListEnvelope get_ai_providers_async(api_version, x_api_version)
Get the available AI providers

Returns every AI provider key this instance has a registered adapter for. The set is a property of the deployment, so it is not tenant-scoped; what varies per tenant is the credential for a provider, which is never returned here.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AiProviderDtoListEnvelope**](AiProviderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

