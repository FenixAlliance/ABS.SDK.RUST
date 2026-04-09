# \SecurityLogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_security_logs_async**](SecurityLogsApi.md#get_security_logs_async) | **GET** /api/v2/SecurityService/SecurityLogs | Get business security logs
[**get_security_logs_count_async**](SecurityLogsApi.md#get_security_logs_count_async) | **GET** /api/v2/SecurityService/SecurityLogs/Count | Get business security logs count



## get_security_logs_async

> models::BusinessSecurityLogDtoListEnvelope get_security_logs_async(tenant_id, api_version, x_api_version)
Get business security logs

Retrieves security logs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessSecurityLogDtoListEnvelope**](BusinessSecurityLogDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_security_logs_count_async

> models::Int32Envelope get_security_logs_count_async(tenant_id, api_version, x_api_version)
Get business security logs count

Retrieves the count of security logs for the specified tenant.

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

