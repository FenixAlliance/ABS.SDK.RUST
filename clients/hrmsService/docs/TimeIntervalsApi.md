# \TimeIntervalsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_time_interval_async**](TimeIntervalsApi.md#create_time_interval_async) | **POST** /api/v2/HrmsService/TimeIntervals | Create a time interval
[**delete_time_interval_async**](TimeIntervalsApi.md#delete_time_interval_async) | **DELETE** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Delete a time interval
[**get_time_interval_by_id_async**](TimeIntervalsApi.md#get_time_interval_by_id_async) | **GET** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Get time interval by ID
[**get_time_intervals_async**](TimeIntervalsApi.md#get_time_intervals_async) | **GET** /api/v2/HrmsService/TimeIntervals | Get time intervals
[**get_time_intervals_count_async**](TimeIntervalsApi.md#get_time_intervals_count_async) | **GET** /api/v2/HrmsService/TimeIntervals/Count | Count time intervals
[**update_time_interval_async**](TimeIntervalsApi.md#update_time_interval_async) | **PUT** /api/v2/HrmsService/TimeIntervals/{timeIntervalId} | Update a time interval



## create_time_interval_async

> models::EmptyEnvelope create_time_interval_async(tenant_id, api_version, x_api_version, time_interval_create_dto)
Create a time interval

Creates a new time interval for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**time_interval_create_dto** | Option<[**TimeIntervalCreateDto**](TimeIntervalCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_time_interval_async

> models::EmptyEnvelope delete_time_interval_async(tenant_id, time_interval_id, api_version, x_api_version)
Delete a time interval

Deletes a time interval for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**time_interval_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_time_interval_by_id_async

> models::TimeIntervalDtoEnvelope get_time_interval_by_id_async(tenant_id, time_interval_id, api_version, x_api_version)
Get time interval by ID

Retrieves a specific time interval by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**time_interval_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TimeIntervalDtoEnvelope**](TimeIntervalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_time_intervals_async

> models::TimeIntervalDtoListEnvelope get_time_intervals_async(tenant_id, api_version, x_api_version)
Get time intervals

Retrieves time intervals for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TimeIntervalDtoListEnvelope**](TimeIntervalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_time_intervals_count_async

> models::Int32Envelope get_time_intervals_count_async(tenant_id, api_version, x_api_version)
Count time intervals

Counts time intervals for the specified tenant.

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


## update_time_interval_async

> models::EmptyEnvelope update_time_interval_async(tenant_id, time_interval_id, api_version, x_api_version, time_interval_update_dto)
Update a time interval

Updates an existing time interval for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**time_interval_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**time_interval_update_dto** | Option<[**TimeIntervalUpdateDto**](TimeIntervalUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

