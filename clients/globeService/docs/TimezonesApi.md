# \TimezonesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_timezones_async**](TimezonesApi.md#count_timezones_async) | **GET** /api/v2/GlobeService/Timezones/Count | Count timezones
[**get_time_zone_by_id_async**](TimezonesApi.md#get_time_zone_by_id_async) | **GET** /api/v2/GlobeService/Timezones/{timeZoneId} | Get timezone by ID
[**get_time_zones_async**](TimezonesApi.md#get_time_zones_async) | **GET** /api/v2/GlobeService/Timezones | Get all timezones



## count_timezones_async

> models::Int32Envelope count_timezones_async(api_version, x_api_version)
Count timezones

Returns the total number of supported timezones, with optional OData filtering.

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


## get_time_zone_by_id_async

> models::TimezoneDtoEnvelope get_time_zone_by_id_async(time_zone_id, api_version, x_api_version)
Get timezone by ID

Retrieves a single timezone by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**time_zone_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TimezoneDtoEnvelope**](TimezoneDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_time_zones_async

> models::TimezoneDtoListEnvelope get_time_zones_async(api_version, x_api_version)
Get all timezones

Retrieves the list of all supported timezones with optional OData pagination and filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TimezoneDtoListEnvelope**](TimezoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

