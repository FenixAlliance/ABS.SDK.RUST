# \OverviewApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_system_overview**](OverviewApi.md#get_system_overview) | **GET** /api/v2/SystemService/Overview | Get system overview information



## get_system_overview

> models::SystemOverviewDtoEnvelope get_system_overview(api_version, x_api_version)
Get system overview information

Returns runtime, memory, and entity count information for the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SystemOverviewDtoEnvelope**](SystemOverviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

