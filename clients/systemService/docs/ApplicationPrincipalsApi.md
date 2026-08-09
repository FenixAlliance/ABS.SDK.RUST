# \ApplicationPrincipalsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**disable_global_application_principal**](ApplicationPrincipalsApi.md#disable_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Disable | Disable an application principal (global)
[**enable_global_application_principal**](ApplicationPrincipalsApi.md#enable_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Enable | Enable an application principal (global)
[**get_global_application_principal**](ApplicationPrincipalsApi.md#get_global_application_principal) | **GET** /api/v2/SystemService/ApplicationPrincipals/{principalId} | Get one application principal (any tenant)
[**get_global_application_principals**](ApplicationPrincipalsApi.md#get_global_application_principals) | **GET** /api/v2/SystemService/ApplicationPrincipals | List application principals across all tenants
[**get_global_application_principals_count**](ApplicationPrincipalsApi.md#get_global_application_principals_count) | **GET** /api/v2/SystemService/ApplicationPrincipals/Count | Count application principals across all tenants
[**grant_global_application_principal_permission**](ApplicationPrincipalsApi.md#grant_global_application_principal_permission) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Permissions | Grant a permission to an application principal (any tenant)
[**provision_global_application_principal**](ApplicationPrincipalsApi.md#provision_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/Provision | Provision an application principal (any tenant, incl. system-locked)
[**provision_payments_connector**](ApplicationPrincipalsApi.md#provision_payments_connector) | **POST** /api/v2/SystemService/ApplicationPrincipals/PaymentsConnector | Provision the platform payments-connector identity
[**revoke_global_application_principal_permission**](ApplicationPrincipalsApi.md#revoke_global_application_principal_permission) | **DELETE** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Permissions/{permission} | Revoke a permission from an application principal (any tenant)
[**suspend_global_application_principal**](ApplicationPrincipalsApi.md#suspend_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Suspend | Suspend an application principal (global)



## disable_global_application_principal

> models::EmptyEnvelope disable_global_application_principal(principal_id, tenant_id, api_version, x_api_version)
Disable an application principal (global)

Disables the application principal; dependent unattended execution fails closed (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## enable_global_application_principal

> models::EmptyEnvelope enable_global_application_principal(principal_id, tenant_id, api_version, x_api_version)
Enable an application principal (global)

Reinstates the application principal to the Active lifecycle state (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_global_application_principal

> models::ApplicationPrincipalDetailDtoEnvelope get_global_application_principal(principal_id, tenant_id, api_version, x_api_version)
Get one application principal (any tenant)

Returns one application principal's detail by id: owning application, an enrollment, the system-locked flag, lifecycle status, and that enrollment's explicit least-privilege grants. Pass tenantId to select the enrollment for a multi-tenant principal; when omitted the principal's first enrollment is used. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## get_global_application_principals

> models::ApplicationPrincipalDtoIReadOnlyListEnvelope get_global_application_principals(api_version, x_api_version, application_principal_dto_collection_query_parameters)
List application principals across all tenants

Lists every non-human application principal enrollment across ALL tenants (payload-safe fields only), including the platform-managed (system-locked) connectors. Use OData to scope — e.g. $filter=SystemLocked eq true for the platform connectors or TenantId eq '{guid}' for one tenant — and to page/order. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**application_principal_dto_collection_query_parameters** | Option<[**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ApplicationPrincipalDtoIReadOnlyListEnvelope**](ApplicationPrincipalDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_global_application_principals_count

> models::Int32Envelope get_global_application_principals_count(api_version, x_api_version, application_principal_dto_collection_query_parameters)
Count application principals across all tenants

Returns the count of application principal enrollments across ALL tenants under the same OData shaping as the list read (e.g. $filter=SystemLocked eq true). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## grant_global_application_principal_permission

> models::EmptyEnvelope grant_global_application_principal_permission(principal_id, tenant_id, application_principal_permission_request_dto, api_version, x_api_version)
Grant a permission to an application principal (any tenant)

Grants a single least-privilege permission to the application principal's enrollment in the tenantId tenant (grants are per-tenant, so tenantId is required). Owner/admin/wildcard/_*_manage permissions are rejected even for a global admin (least-privilege by construction). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## provision_global_application_principal

> models::ApplicationPrincipalProvisioningResultDtoEnvelope provision_global_application_principal(application_principal_provision_request_dto, tenant_id, api_version, x_api_version)
Provision an application principal (any tenant, incl. system-locked)

Idempotently provisions the application principal (and its own least-privilege enrollment) for a governed business application. tenantId selects the target tenant (defaults to the platform/root tenant). Unlike the per-tenant lane, a system-locked platform application is provisionable here. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**application_principal_provision_request_dto** | [**ApplicationPrincipalProvisionRequestDto**](ApplicationPrincipalProvisionRequestDto.md) |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## provision_payments_connector

> models::ApplicationPrincipalProvisioningResultDtoEnvelope provision_payments_connector(tenant_id, api_version, x_api_version)
Provision the platform payments-connector identity

Idempotently stands up the platform payments-connector identity — its well-known business application, its application principal, and its own least-privilege enrollment (payments_create/payments_update/journals_post). tenantId selects the target tenant (defaults to the platform/root tenant). The provisioned connector then appears in this global list and (for its tenant) the per-tenant list. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ApplicationPrincipalProvisioningResultDtoEnvelope**](ApplicationPrincipalProvisioningResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## revoke_global_application_principal_permission

> models::EmptyEnvelope revoke_global_application_principal_permission(principal_id, permission, tenant_id, api_version, x_api_version)
Revoke a permission from an application principal (any tenant)

Revokes a direct permission grant from the application principal's enrollment in the tenantId tenant (required). Idempotent. Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**permission** | **String** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## suspend_global_application_principal

> models::EmptyEnvelope suspend_global_application_principal(principal_id, tenant_id, api_version, x_api_version)
Suspend an application principal (global)

Temporarily suspends the application principal; its identity is retained but it cannot act until reinstated (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**principal_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
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

