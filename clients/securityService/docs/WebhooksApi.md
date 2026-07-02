# \WebhooksApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_webhook_requests_async**](WebhooksApi.md#get_webhook_requests_async) | **GET** /api/v2/SecurityService/Webhooks | Get all webhook requests
[**get_webhook_requests_count_async**](WebhooksApi.md#get_webhook_requests_count_async) | **GET** /api/v2/SecurityService/Webhooks/Count | Get webhook requests count



## get_webhook_requests_async

> models::WebhookRequestDtoListEnvelope get_webhook_requests_async(tenant_id, api_version, x_api_version)
Get all webhook requests

Retrieves all webhook requests for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebhookRequestDtoListEnvelope**](WebhookRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhook_requests_count_async

> models::Int32Envelope get_webhook_requests_count_async(tenant_id, api_version, x_api_version)
Get webhook requests count

Retrieves the count of webhook requests for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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

