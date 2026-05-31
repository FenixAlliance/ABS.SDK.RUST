# \ApplicationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_application**](ApplicationsApi.md#get_application) | **GET** /api/v2/Applications/{appId} | Get application by ID
[**get_granted_enrollment_permissions**](ApplicationsApi.md#get_granted_enrollment_permissions) | **GET** /api/v2/Applications/{appId}/GrantedRoles/{securityRoleId}/GrantedPermissions | Get granted permissions for an application role
[**get_granted_tenant_permissions**](ApplicationsApi.md#get_granted_tenant_permissions) | **GET** /api/v2/Applications/{appId}/GrantedPermissions | Get granted tenant permissions for an application
[**get_granted_tenant_roles**](ApplicationsApi.md#get_granted_tenant_roles) | **GET** /api/v2/Applications/{appId}/GrantedRoles | Get granted tenant roles for an application
[**get_required_permissions**](ApplicationsApi.md#get_required_permissions) | **GET** /api/v2/Applications/{appId}/RequiredPermissions | Get required permissions for an application



## get_application

> get_application(app_id, api_version, x_api_version)
Get application by ID

Retrieves an application by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_granted_enrollment_permissions

> get_granted_enrollment_permissions(app_id, security_role_id, enrollment_id, api_version, x_api_version)
Get granted permissions for an application role

Retrieves the list of permissions granted through a specific security role for the specified application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** |  | [required] |
**security_role_id** | **String** |  | [required] |
**enrollment_id** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_granted_tenant_permissions

> get_granted_tenant_permissions(app_id, tenant_id, api_version, x_api_version)
Get granted tenant permissions for an application

Retrieves the list of permissions granted to the specified application within a tenant context.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** |  | [required] |
**tenant_id** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_granted_tenant_roles

> get_granted_tenant_roles(app_id, tenant_id, api_version, x_api_version)
Get granted tenant roles for an application

Retrieves the list of security roles granted to the specified application within a tenant context.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** |  | [required] |
**tenant_id** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_required_permissions

> get_required_permissions(app_id, api_version, x_api_version)
Get required permissions for an application

Retrieves the list of permissions required by the specified application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**app_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

