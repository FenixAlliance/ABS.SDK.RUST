# \TrackingPixelsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tracking_pixel_async**](TrackingPixelsApi.md#get_tracking_pixel_async) | **GET** /api/v2/MarketingService/TrackingPixels/{pixelId} | Get a tracking pixel



## get_tracking_pixel_async

> models::OrderDtoEnvelope get_tracking_pixel_async(pixel_id, api_version, x_api_version)
Get a tracking pixel

Retrieves a tracking pixel by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pixel_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

