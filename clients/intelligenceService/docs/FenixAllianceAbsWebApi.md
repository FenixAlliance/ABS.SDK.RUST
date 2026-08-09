# \FenixAllianceAbsWebApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_logout_post**](FenixAllianceAbsWebApi.md#account_logout_post) | **POST** /Account/Logout | 
[**account_manage_download_personal_data_post**](FenixAllianceAbsWebApi.md#account_manage_download_personal_data_post) | **POST** /Account/Manage/DownloadPersonalData | 
[**account_manage_link_external_login_post**](FenixAllianceAbsWebApi.md#account_manage_link_external_login_post) | **POST** /Account/Manage/LinkExternalLogin | 
[**account_perform_external_login_post**](FenixAllianceAbsWebApi.md#account_perform_external_login_post) | **POST** /Account/PerformExternalLogin | 
[**forgot_password_post**](FenixAllianceAbsWebApi.md#forgot_password_post) | **POST** /forgotPassword | 
[**health_get**](FenixAllianceAbsWebApi.md#health_get) | **GET** /health | 
[**hello_get**](FenixAllianceAbsWebApi.md#hello_get) | **GET** /hello | 
[**login_post**](FenixAllianceAbsWebApi.md#login_post) | **POST** /login | 
[**manage2fa_post**](FenixAllianceAbsWebApi.md#manage2fa_post) | **POST** /manage/2fa | 
[**manage_info_get**](FenixAllianceAbsWebApi.md#manage_info_get) | **GET** /manage/info | 
[**manage_info_post**](FenixAllianceAbsWebApi.md#manage_info_post) | **POST** /manage/info | 
[**map_identity_api_slash_confirm_email**](FenixAllianceAbsWebApi.md#map_identity_api_slash_confirm_email) | **GET** /confirmEmail | 
[**refresh_post**](FenixAllianceAbsWebApi.md#refresh_post) | **POST** /refresh | 
[**register_post**](FenixAllianceAbsWebApi.md#register_post) | **POST** /register | 
[**resend_confirmation_email_post**](FenixAllianceAbsWebApi.md#resend_confirmation_email_post) | **POST** /resendConfirmationEmail | 
[**reset_password_post**](FenixAllianceAbsWebApi.md#reset_password_post) | **POST** /resetPassword | 
[**version_get**](FenixAllianceAbsWebApi.md#version_get) | **GET** /version | 



## account_logout_post

> account_logout_post(return_url)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**return_url** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_manage_download_personal_data_post

> account_manage_download_personal_data_post()


### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_manage_link_external_login_post

> account_manage_link_external_login_post(provider)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**provider** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_perform_external_login_post

> account_perform_external_login_post(provider, return_url)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**provider** | Option<**String**> |  |  |
**return_url** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## forgot_password_post

> forgot_password_post(forgot_password_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**forgot_password_request** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## health_get

> health_get()


### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## hello_get

> hello_get()


### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## login_post

> models::AccessTokenResponse login_post(login_request, use_cookies, use_session_cookies)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**login_request** | [**LoginRequest**](LoginRequest.md) |  | [required] |
**use_cookies** | Option<**bool**> |  |  |
**use_session_cookies** | Option<**bool**> |  |  |

### Return type

[**models::AccessTokenResponse**](AccessTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## manage2fa_post

> models::TwoFactorResponse manage2fa_post(two_factor_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**two_factor_request** | [**TwoFactorRequest**](TwoFactorRequest.md) |  | [required] |

### Return type

[**models::TwoFactorResponse**](TwoFactorResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## manage_info_get

> models::InfoResponse manage_info_get()


### Parameters

This endpoint does not need any parameter.

### Return type

[**models::InfoResponse**](InfoResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## manage_info_post

> models::InfoResponse manage_info_post(info_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**info_request** | [**InfoRequest**](InfoRequest.md) |  | [required] |

### Return type

[**models::InfoResponse**](InfoResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## map_identity_api_slash_confirm_email

> map_identity_api_slash_confirm_email(user_id, code, changed_email)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **String** |  | [required] |
**code** | **String** |  | [required] |
**changed_email** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## refresh_post

> models::AccessTokenResponse refresh_post(refresh_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**refresh_request** | [**RefreshRequest**](RefreshRequest.md) |  | [required] |

### Return type

[**models::AccessTokenResponse**](AccessTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## register_post

> register_post(register_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**register_request** | [**RegisterRequest**](RegisterRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## resend_confirmation_email_post

> resend_confirmation_email_post(resend_confirmation_email_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**resend_confirmation_email_request** | [**ResendConfirmationEmailRequest**](ResendConfirmationEmailRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## reset_password_post

> reset_password_post(reset_password_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**reset_password_request** | [**ResetPasswordRequest**](ResetPasswordRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## version_get

> version_get()


### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

