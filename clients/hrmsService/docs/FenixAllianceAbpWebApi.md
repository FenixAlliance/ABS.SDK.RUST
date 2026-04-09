# \FenixAllianceAbpWebApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**forgot_password_post**](FenixAllianceAbpWebApi.md#forgot_password_post) | **POST** /forgotPassword | 
[**health_get**](FenixAllianceAbpWebApi.md#health_get) | **GET** /health | 
[**hello_get**](FenixAllianceAbpWebApi.md#hello_get) | **GET** /hello | 
[**login_post**](FenixAllianceAbpWebApi.md#login_post) | **POST** /login | 
[**manage2fa_post**](FenixAllianceAbpWebApi.md#manage2fa_post) | **POST** /manage/2fa | 
[**manage_info_get**](FenixAllianceAbpWebApi.md#manage_info_get) | **GET** /manage/info | 
[**manage_info_post**](FenixAllianceAbpWebApi.md#manage_info_post) | **POST** /manage/info | 
[**map_identity_api_slash_confirm_email**](FenixAllianceAbpWebApi.md#map_identity_api_slash_confirm_email) | **GET** /confirmEmail | 
[**refresh_post**](FenixAllianceAbpWebApi.md#refresh_post) | **POST** /refresh | 
[**register_post**](FenixAllianceAbpWebApi.md#register_post) | **POST** /register | 
[**resend_confirmation_email_post**](FenixAllianceAbpWebApi.md#resend_confirmation_email_post) | **POST** /resendConfirmationEmail | 
[**reset_password_post**](FenixAllianceAbpWebApi.md#reset_password_post) | **POST** /resetPassword | 
[**version_get**](FenixAllianceAbpWebApi.md#version_get) | **GET** /version | 



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

