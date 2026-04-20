# \OAuthApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_password_sign_in_async**](OAuthApi.md#check_password_sign_in_async) | **GET** /api/v2/OAuth/SignIn | Check password sign-in
[**get**](OAuthApi.md#get) | **GET** /api/v2/OAuth/WhoAmI | Get current user identity
[**get_jw_ks**](OAuthApi.md#get_jw_ks) | **GET** /api/v2/OAuth/{applicationId}/Keys | Get JSON Web Key Set
[**get_open_id_configuration**](OAuthApi.md#get_open_id_configuration) | **GET** /api/v2/OAuth/{tenantId}/{applicationId}/.Well-Known/OpenId-Configuration | Get OpenID configuration
[**get_permissions**](OAuthApi.md#get_permissions) | **GET** /api/v2/OAuth/Permissions | Get user permissions
[**password_sign_in_async**](OAuthApi.md#password_sign_in_async) | **POST** /api/v2/OAuth/SignIn | Sign in with password
[**token**](OAuthApi.md#token) | **POST** /api/v2/OAuth/Token | Get OAuth token



## check_password_sign_in_async

> models::UserCreateDtoEnvelope check_password_sign_in_async(api_version, x_api_version)
Check password sign-in

Verifies sign-in credentials and returns user details without creating a session.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserCreateDtoEnvelope**](UserCreateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get

> models::AuthorizationResultEnvelope get(tenant_id, api_version, x_api_version)
Get current user identity

Returns the authorization result for the authenticated user, including identity and tenant context.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AuthorizationResultEnvelope**](AuthorizationResultEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_jw_ks

> models::JsonWebKeySetEnvelope get_jw_ks(application_id, api_version, x_api_version)
Get JSON Web Key Set

Retrieves the signing keys (JWKS) for a specific application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**application_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JsonWebKeySetEnvelope**](JsonWebKeySetEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_open_id_configuration

> models::OpenIdConfigurationEnvelope get_open_id_configuration(tenant_id, application_id, api_version, x_api_version)
Get OpenID configuration

Retrieves the OpenID Connect discovery document for a specific application within a tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OpenIdConfigurationEnvelope**](OpenIdConfigurationEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_permissions

> models::StringListEnvelope get_permissions(tenant_id, user_id, api_version, x_api_version)
Get user permissions

Retrieves the list of permission identifiers for a specific user within a tenant context.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**user_id** | Option<**String**> |  |  |
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


## password_sign_in_async

> models::JsonWebTokenEnvelope password_sign_in_async(api_version, x_api_version, signin_model)
Sign in with password

Authenticates a user using email and password credentials.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signin_model** | Option<[**SigninModel**](SigninModel.md)> |  |  |

### Return type

[**models::JsonWebTokenEnvelope**](JsonWebTokenEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## token

> models::JsonWebTokenEnvelope token(api_version, x_api_version, o_auth_token_request)
Get OAuth token

Generates an OAuth token based on the provided credentials or grant type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**o_auth_token_request** | Option<[**OAuthTokenRequest**](OAuthTokenRequest.md)> |  |  |

### Return type

[**models::JsonWebTokenEnvelope**](JsonWebTokenEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

