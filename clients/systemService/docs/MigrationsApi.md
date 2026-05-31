# \MigrationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**migrate**](MigrationsApi.md#migrate) | **POST** /api/v2/SystemService/Migrations/Migrate | Apply pending database migrations
[**migrations**](MigrationsApi.md#migrations) | **GET** /api/v2/SystemService/Migrations | Retrieve database migrations



## migrate

> models::StringListEnvelope migrate(api_version, x_api_version)
Apply pending database migrations

Applies all pending database migrations and returns the list of migrations that were applied.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## migrations

> models::StringListEnvelope migrations(pending, api_version, x_api_version)
Retrieve database migrations

Retrieves the list of applied or pending database migrations.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pending** | Option<**bool**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

