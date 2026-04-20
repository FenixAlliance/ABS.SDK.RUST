# \OAuthApplicationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_o_auth_application_async**](OAuthApplicationsApi.md#create_o_auth_application_async) | **POST** /api/v2/SecurityService/OAuthApplications | Create a new OAuth application
[**delete_o_auth_application_async**](OAuthApplicationsApi.md#delete_o_auth_application_async) | **DELETE** /api/v2/SecurityService/OAuthApplications/{applicationId} | Delete an OAuth application
[**get_o_auth_application_by_id_async**](OAuthApplicationsApi.md#get_o_auth_application_by_id_async) | **GET** /api/v2/SecurityService/OAuthApplications/{applicationId} | Get OAuth application by ID
[**get_o_auth_applications_async**](OAuthApplicationsApi.md#get_o_auth_applications_async) | **GET** /api/v2/SecurityService/OAuthApplications | Get all OAuth applications
[**get_o_auth_applications_count_async**](OAuthApplicationsApi.md#get_o_auth_applications_count_async) | **GET** /api/v2/SecurityService/OAuthApplications/Count | Get OAuth applications count
[**get_o_auth_authorization_by_id_async**](OAuthApplicationsApi.md#get_o_auth_authorization_by_id_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations/{authorizationId} | Get OAuth authorization by ID
[**get_o_auth_authorizations_async**](OAuthApplicationsApi.md#get_o_auth_authorizations_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations | Get all OAuth authorizations
[**get_o_auth_authorizations_count_async**](OAuthApplicationsApi.md#get_o_auth_authorizations_count_async) | **GET** /api/v2/SecurityService/OAuthApplications/Authorizations/Count | Get OAuth authorizations count
[**update_o_auth_application_async**](OAuthApplicationsApi.md#update_o_auth_application_async) | **PUT** /api/v2/SecurityService/OAuthApplications/{applicationId} | Update an existing OAuth application



## create_o_auth_application_async

> models::EmptyEnvelope create_o_auth_application_async(tenant_id, o_auth_application_create_dto, api_version, x_api_version)
Create a new OAuth application

Creates a new OAuth application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**o_auth_application_create_dto** | [**OAuthApplicationCreateDto**](OAuthApplicationCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_o_auth_application_async

> models::EmptyEnvelope delete_o_auth_application_async(tenant_id, application_id, api_version, x_api_version)
Delete an OAuth application

Deletes an existing OAuth application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
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


## get_o_auth_application_by_id_async

> models::OAuthApplicationDtoEnvelope get_o_auth_application_by_id_async(tenant_id, application_id, api_version, x_api_version)
Get OAuth application by ID

Retrieves a specific OAuth application by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OAuthApplicationDtoEnvelope**](OAuthApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_o_auth_applications_async

> models::OAuthApplicationDtoListEnvelope get_o_auth_applications_async(tenant_id, api_version, x_api_version)
Get all OAuth applications

Retrieves all OAuth applications for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OAuthApplicationDtoListEnvelope**](OAuthApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_o_auth_applications_count_async

> models::Int32Envelope get_o_auth_applications_count_async(tenant_id, api_version, x_api_version)
Get OAuth applications count

Retrieves the count of OAuth applications for the specified tenant.

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


## get_o_auth_authorization_by_id_async

> models::OAuthAuthorizationDtoEnvelope get_o_auth_authorization_by_id_async(tenant_id, authorization_id, api_version, x_api_version)
Get OAuth authorization by ID

Retrieves a specific OAuth authorization by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**authorization_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OAuthAuthorizationDtoEnvelope**](OAuthAuthorizationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_o_auth_authorizations_async

> models::OAuthAuthorizationDtoListEnvelope get_o_auth_authorizations_async(tenant_id, user_id, api_version, x_api_version)
Get all OAuth authorizations

Retrieves all OAuth authorizations for the specified user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**user_id** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OAuthAuthorizationDtoListEnvelope**](OAuthAuthorizationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_o_auth_authorizations_count_async

> models::Int32Envelope get_o_auth_authorizations_count_async(tenant_id, user_id, api_version, x_api_version)
Get OAuth authorizations count

Retrieves the count of OAuth authorizations for the specified user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**user_id** | Option<**String**> |  |  |
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


## update_o_auth_application_async

> models::EmptyEnvelope update_o_auth_application_async(tenant_id, application_id, o_auth_application_update_dto, api_version, x_api_version)
Update an existing OAuth application

Updates an existing OAuth application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
**o_auth_application_update_dto** | [**OAuthApplicationUpdateDto**](OAuthApplicationUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

