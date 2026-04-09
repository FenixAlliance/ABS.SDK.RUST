# \RolesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**assign_permission_to_role_async**](RolesApi.md#assign_permission_to_role_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions/{securityPermissionId} | Assign a permission to a role
[**assign_role_to_business_application_async**](RolesApi.md#assign_role_to_business_application_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Applications/{applicationId} | Assign a role to a business application
[**assign_role_to_enrollment_async**](RolesApi.md#assign_role_to_enrollment_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments/{enrollmentId} | Assign a role to an enrollment
[**create_role_async**](RolesApi.md#create_role_async) | **POST** /api/v2/SecurityService/Roles | Create a new role
[**delete_role_async**](RolesApi.md#delete_role_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId} | Delete an existing role
[**get_applications_by_role_async**](RolesApi.md#get_applications_by_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Applications | Get applications by role
[**get_enrollments_by_role_async**](RolesApi.md#get_enrollments_by_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments | Get enrollments by role
[**get_role_async**](RolesApi.md#get_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId} | Get role by ID
[**get_role_permissions_async**](RolesApi.md#get_role_permissions_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions | Get permissions by role
[**get_roles_async**](RolesApi.md#get_roles_async) | **GET** /api/v2/SecurityService/Roles | Get all roles
[**get_roles_by_enrollment_async**](RolesApi.md#get_roles_by_enrollment_async) | **GET** /api/v2/SecurityService/Roles/ByEnrollment/{enrollmentId} | Get roles by enrollment
[**get_roles_count_async**](RolesApi.md#get_roles_count_async) | **GET** /api/v2/SecurityService/Roles/Count | Get roles count
[**revoke_permission_from_role_async**](RolesApi.md#revoke_permission_from_role_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions/{securityPermissionId} | Revoke a permission from a role
[**revoke_role_from_business_application_async**](RolesApi.md#revoke_role_from_business_application_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Applications/{applicationId} | Revoke a role from a business application
[**revoke_role_from_enrollment_async**](RolesApi.md#revoke_role_from_enrollment_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments/{enrollmentId} | Revoke a role from an enrollment
[**update_role_async**](RolesApi.md#update_role_async) | **PUT** /api/v2/SecurityService/Roles/{securityRoleId} | Update an existing role



## assign_permission_to_role_async

> models::EmptyEnvelope assign_permission_to_role_async(tenant_id, security_role_id, security_permission_id, api_version, x_api_version)
Assign a permission to a role

Assigns a security permission to a security role.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## assign_role_to_business_application_async

> models::EmptyEnvelope assign_role_to_business_application_async(tenant_id, security_role_id, application_id, api_version, x_api_version)
Assign a role to a business application

Assigns a security role to a business application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**application_id** | **uuid::Uuid** |  | [required] |
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


## assign_role_to_enrollment_async

> models::EmptyEnvelope assign_role_to_enrollment_async(tenant_id, security_role_id, enrollment_id, api_version, x_api_version)
Assign a role to an enrollment

Assigns a security role to a tenant enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**enrollment_id** | **String** |  | [required] |
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


## create_role_async

> models::EmptyEnvelope create_role_async(tenant_id, security_role_create_dto, api_version, x_api_version)
Create a new role

Creates a new security role for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_create_dto** | [**SecurityRoleCreateDto**](SecurityRoleCreateDto.md) |  | [required] |
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


## delete_role_async

> models::EmptyEnvelope delete_role_async(tenant_id, security_role_id, api_version, x_api_version)
Delete an existing role

Deletes an existing security role for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
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


## get_applications_by_role_async

> models::BusinessApplicationSimpleDtoListEnvelope get_applications_by_role_async(tenant_id, security_role_id, api_version, x_api_version)
Get applications by role

Retrieves all business applications that have a specific role granted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessApplicationSimpleDtoListEnvelope**](BusinessApplicationSimpleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollments_by_role_async

> models::TenantEnrollmentDtoListEnvelope get_enrollments_by_role_async(tenant_id, security_role_id, api_version, x_api_version)
Get enrollments by role

Retrieves all tenant enrollments that have a specific role.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_role_async

> models::SecurityRoleDtoEnvelope get_role_async(tenant_id, security_role_id, api_version, x_api_version)
Get role by ID

Retrieves a specific security role by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SecurityRoleDtoEnvelope**](SecurityRoleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_role_permissions_async

> models::SecurityPermissionDtoListEnvelope get_role_permissions_async(tenant_id, security_role_id, api_version, x_api_version)
Get permissions by role

Retrieves all security permissions assigned to a specific role.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SecurityPermissionDtoListEnvelope**](SecurityPermissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_roles_async

> models::SecurityRoleDtoListEnvelope get_roles_async(tenant_id, api_version, x_api_version)
Get all roles

Retrieves all security roles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_roles_by_enrollment_async

> models::SecurityRoleDtoListEnvelope get_roles_by_enrollment_async(tenant_id, enrollment_id, api_version, x_api_version)
Get roles by enrollment

Retrieves all security roles granted to a specific enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_roles_count_async

> models::Int32Envelope get_roles_count_async(tenant_id, api_version, x_api_version)
Get roles count

Retrieves the count of security roles for the specified tenant.

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


## revoke_permission_from_role_async

> models::EmptyEnvelope revoke_permission_from_role_async(tenant_id, security_role_id, security_permission_id, api_version, x_api_version)
Revoke a permission from a role

Revokes a security permission from a security role.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## revoke_role_from_business_application_async

> models::EmptyEnvelope revoke_role_from_business_application_async(tenant_id, security_role_id, application_id, api_version, x_api_version)
Revoke a role from a business application

Revokes a security role from a business application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**application_id** | **uuid::Uuid** |  | [required] |
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


## revoke_role_from_enrollment_async

> models::EmptyEnvelope revoke_role_from_enrollment_async(tenant_id, security_role_id, enrollment_id, api_version, x_api_version)
Revoke a role from an enrollment

Revokes a security role from a tenant enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**enrollment_id** | **String** |  | [required] |
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


## update_role_async

> models::EmptyEnvelope update_role_async(tenant_id, security_role_id, security_role_update_dto, api_version, x_api_version)
Update an existing role

Updates an existing security role for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_role_id** | **String** |  | [required] |
**security_role_update_dto** | [**SecurityRoleUpdateDto**](SecurityRoleUpdateDto.md) |  | [required] |
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

