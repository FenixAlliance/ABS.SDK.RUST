# \ApplicationPrincipalsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**disable_application_principal_async**](ApplicationPrincipalsApi.md#disable_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Disable | Disable an application principal
[**enable_application_principal_async**](ApplicationPrincipalsApi.md#enable_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Enable | Enable an application principal
[**get_application_principal_async**](ApplicationPrincipalsApi.md#get_application_principal_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals/{principalId} | Get application principal by ID
[**get_application_principals_async**](ApplicationPrincipalsApi.md#get_application_principals_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals | Get all application principals
[**get_application_principals_count_async**](ApplicationPrincipalsApi.md#get_application_principals_count_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals/Count | Get application principals count
[**grant_permission_async**](ApplicationPrincipalsApi.md#grant_permission_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Permissions | Grant a permission to an application principal
[**provision_application_principal_async**](ApplicationPrincipalsApi.md#provision_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/Provision | Provision an application principal
[**revoke_permission_async**](ApplicationPrincipalsApi.md#revoke_permission_async) | **DELETE** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Permissions/{permission} | Revoke a permission from an application principal
[**suspend_application_principal_async**](ApplicationPrincipalsApi.md#suspend_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Suspend | Suspend an application principal



## disable_application_principal_async

> models::EmptyEnvelope disable_application_principal_async(tenant_id, principal_id, api_version, x_api_version)
Disable an application principal

Disables the application principal; dependent unattended execution fails closed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
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


## enable_application_principal_async

> models::EmptyEnvelope enable_application_principal_async(tenant_id, principal_id, api_version, x_api_version)
Enable an application principal

Reinstates the application principal to the Active lifecycle state.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
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


## get_application_principal_async

> models::ApplicationPrincipalDetailDtoEnvelope get_application_principal_async(tenant_id, principal_id, api_version, x_api_version)
Get application principal by ID

Retrieves a specific application principal: owning application, tenant enrollment, lifecycle status, system-locked flag, and its explicit least-privilege permission grants.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ApplicationPrincipalDetailDtoEnvelope**](ApplicationPrincipalDetailDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_application_principals_async

> models::ApplicationPrincipalDtoListEnvelope get_application_principals_async(tenant_id, api_version, x_api_version, application_principal_dto_collection_query_parameters)
Get all application principals

Retrieves the non-human application principals enrolled in the specified tenant (including read-only system-locked platform principals).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**application_principal_dto_collection_query_parameters** | Option<[**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ApplicationPrincipalDtoListEnvelope**](ApplicationPrincipalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_application_principals_count_async

> models::Int32Envelope get_application_principals_count_async(tenant_id, api_version, x_api_version, application_principal_dto_collection_query_parameters)
Get application principals count

Retrieves the count of application principals enrolled in the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**application_principal_dto_collection_query_parameters** | Option<[**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## grant_permission_async

> models::EmptyEnvelope grant_permission_async(tenant_id, principal_id, application_principal_permission_request_dto, api_version, x_api_version)
Grant a permission to an application principal

Grants a single least-privilege permission to the application principal's enrollment. Owner/admin/wildcard/_*_manage permissions are rejected; system-locked principals require a platform administrator.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
**application_principal_permission_request_dto** | [**ApplicationPrincipalPermissionRequestDto**](ApplicationPrincipalPermissionRequestDto.md) |  | [required] |
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


## provision_application_principal_async

> models::ApplicationPrincipalProvisioningResultDtoEnvelope provision_application_principal_async(tenant_id, application_principal_provision_request_dto, api_version, x_api_version)
Provision an application principal

Idempotently provisions the application principal (and its own least-privilege enrollment) for a governed business application in the specified tenant. System-locked platform applications require a platform administrator.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_principal_provision_request_dto** | [**ApplicationPrincipalProvisionRequestDto**](ApplicationPrincipalProvisionRequestDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ApplicationPrincipalProvisioningResultDtoEnvelope**](ApplicationPrincipalProvisioningResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## revoke_permission_async

> models::EmptyEnvelope revoke_permission_async(tenant_id, principal_id, permission, api_version, x_api_version)
Revoke a permission from an application principal

Revokes a direct permission grant from the application principal's enrollment. System-locked principals require a platform administrator.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
**permission** | **String** |  | [required] |
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


## suspend_application_principal_async

> models::EmptyEnvelope suspend_application_principal_async(tenant_id, principal_id, api_version, x_api_version)
Suspend an application principal

Temporarily suspends the application principal; its identity is retained but it cannot act until reinstated.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**principal_id** | **uuid::Uuid** |  | [required] |
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

