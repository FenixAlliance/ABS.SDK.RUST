# \EmailsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**admin_preview_basic_email_template**](EmailsApi.md#admin_preview_basic_email_template) | **POST** /api/v2/SystemService/Emails/Preview | Preview a rendered basic email template.
[**admin_send_basic_email**](EmailsApi.md#admin_send_basic_email) | **POST** /api/v2/SystemService/Emails/SendBasic | Send a basic transactional email to recipients.



## admin_preview_basic_email_template

> admin_preview_basic_email_template(api_version, x_api_version, object_email_dispatch_request)
Preview a rendered basic email template.

This action is only available for global administrators (business_owner role).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**object_email_dispatch_request** | Option<[**ObjectEmailDispatchRequest**](ObjectEmailDispatchRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## admin_send_basic_email

> models::TenantDtoListEnvelope admin_send_basic_email(api_version, x_api_version, object_email_dispatch_request)
Send a basic transactional email to recipients.

This action is only available for global administrators (business_owner role).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**object_email_dispatch_request** | Option<[**ObjectEmailDispatchRequest**](ObjectEmailDispatchRequest.md)> |  |  |

### Return type

[**models::TenantDtoListEnvelope**](TenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

