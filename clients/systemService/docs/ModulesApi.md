# \ModulesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_modules**](ModulesApi.md#get_all_modules) | **GET** /api/v2/StudioService/Modules | Get all modules available on this suite server instance.
[**get_available_modules**](ModulesApi.md#get_available_modules) | **GET** /api/v2/StudioService/Modules/Data | Get all modules available to a tenant user.



## get_all_modules

> models::StudioModuleListEnvelope get_all_modules(tenant_id, api_version, x_api_version)
Get all modules available on this suite server instance.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::StudioModuleListEnvelope**](StudioModuleListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_available_modules

> models::ModuleListEnvelope get_available_modules(tenant_id, api_version, x_api_version)
Get all modules available to a tenant user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ModuleListEnvelope**](ModuleListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

