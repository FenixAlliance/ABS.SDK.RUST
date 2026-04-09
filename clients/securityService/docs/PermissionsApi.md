# \PermissionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**assign_permission_to_business_application_async**](PermissionsApi.md#assign_permission_to_business_application_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications/{applicationId} | Assign a permission to a business application
[**assign_permission_to_enrollment_async**](PermissionsApi.md#assign_permission_to_enrollment_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments/{enrollmentId} | Assign a permission to an enrollment
[**assign_role_to_permission_async**](PermissionsApi.md#assign_role_to_permission_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles/{securityRoleId} | Assign a role to a permission
[**create_permission_async**](PermissionsApi.md#create_permission_async) | **POST** /api/v2/SecurityService/Permissions | Create a new permission
[**delete_permission_async**](PermissionsApi.md#delete_permission_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId} | Delete an existing permission
[**get_applications_by_permission_async**](PermissionsApi.md#get_applications_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications | Get applications by permission
[**get_enrollments_by_permission_async**](PermissionsApi.md#get_enrollments_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments | Get enrollments by permission
[**get_permission_async**](PermissionsApi.md#get_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId} | Get permission by ID
[**get_permissions_async**](PermissionsApi.md#get_permissions_async) | **GET** /api/v2/SecurityService/Permissions | Get all permissions
[**get_permissions_by_enrollment_async**](PermissionsApi.md#get_permissions_by_enrollment_async) | **GET** /api/v2/SecurityService/Permissions/ByEnrollment/{enrollmentId} | Get permissions by enrollment
[**get_permissions_count_async**](PermissionsApi.md#get_permissions_count_async) | **GET** /api/v2/SecurityService/Permissions/Count | Get permissions count
[**get_roles_by_permission_async**](PermissionsApi.md#get_roles_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles | Get roles by permission
[**revoke_permission_from_business_application_async**](PermissionsApi.md#revoke_permission_from_business_application_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications/{applicationId} | Revoke a permission from a business application
[**revoke_permission_from_enrollment_async**](PermissionsApi.md#revoke_permission_from_enrollment_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments/{enrollmentId} | Revoke a permission from an enrollment
[**revoke_role_from_permission_async**](PermissionsApi.md#revoke_role_from_permission_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles/{securityRoleId} | Revoke a role from a permission
[**update_permission_async**](PermissionsApi.md#update_permission_async) | **PUT** /api/v2/SecurityService/Permissions/{securityPermissionId} | Update an existing permission



## assign_permission_to_business_application_async

> models::EmptyEnvelope assign_permission_to_business_application_async(tenant_id, security_permission_id, application_id, api_version, x_api_version)
Assign a permission to a business application

Assigns a security permission to a business application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## assign_permission_to_enrollment_async

> models::EmptyEnvelope assign_permission_to_enrollment_async(tenant_id, security_permission_id, enrollment_id, api_version, x_api_version)
Assign a permission to an enrollment

Assigns a security permission to a tenant enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## assign_role_to_permission_async

> models::EmptyEnvelope assign_role_to_permission_async(tenant_id, security_permission_id, security_role_id, api_version, x_api_version)
Assign a role to a permission

Assigns a security role to a security permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## create_permission_async

> models::EmptyEnvelope create_permission_async(tenant_id, security_permission_create_dto, api_version, x_api_version)
Create a new permission

Creates a new security permission for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_create_dto** | [**SecurityPermissionCreateDto**](SecurityPermissionCreateDto.md) |  | [required] |
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


## delete_permission_async

> models::EmptyEnvelope delete_permission_async(tenant_id, security_permission_id, api_version, x_api_version)
Delete an existing permission

Deletes an existing security permission for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_applications_by_permission_async

> models::BusinessApplicationSimpleDtoListEnvelope get_applications_by_permission_async(tenant_id, security_permission_id, api_version, x_api_version)
Get applications by permission

Retrieves all business applications that have a specific permission granted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## get_enrollments_by_permission_async

> models::TenantEnrollmentDtoListEnvelope get_enrollments_by_permission_async(tenant_id, security_permission_id, api_version, x_api_version)
Get enrollments by permission

Retrieves all tenant enrollments that have a specific permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## get_permission_async

> models::SecurityPermissionDtoEnvelope get_permission_async(tenant_id, security_permission_id, api_version, x_api_version)
Get permission by ID

Retrieves a specific security permission by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SecurityPermissionDtoEnvelope**](SecurityPermissionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_permissions_async

> models::SecurityPermissionDtoListEnvelope get_permissions_async(tenant_id, api_version, x_api_version)
Get all permissions

Retrieves all security permissions for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_permissions_by_enrollment_async

> models::SecurityPermissionDtoListEnvelope get_permissions_by_enrollment_async(tenant_id, enrollment_id, api_version, x_api_version)
Get permissions by enrollment

Retrieves all security permissions granted to a specific enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **String** |  | [required] |
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


## get_permissions_count_async

> models::Int32Envelope get_permissions_count_async(tenant_id, api_version, x_api_version)
Get permissions count

Retrieves the count of security permissions for the specified tenant.

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


## get_roles_by_permission_async

> models::SecurityRoleDtoListEnvelope get_roles_by_permission_async(tenant_id, security_permission_id, api_version, x_api_version)
Get roles by permission

Retrieves all security roles that have a specific permission granted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## revoke_permission_from_business_application_async

> models::EmptyEnvelope revoke_permission_from_business_application_async(tenant_id, security_permission_id, application_id, api_version, x_api_version)
Revoke a permission from a business application

Revokes a security permission from a business application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## revoke_permission_from_enrollment_async

> models::EmptyEnvelope revoke_permission_from_enrollment_async(tenant_id, security_permission_id, enrollment_id, api_version, x_api_version)
Revoke a permission from an enrollment

Revokes a security permission from a tenant enrollment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## revoke_role_from_permission_async

> models::EmptyEnvelope revoke_role_from_permission_async(tenant_id, security_permission_id, security_role_id, api_version, x_api_version)
Revoke a role from a permission

Revokes a security role from a security permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
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


## update_permission_async

> models::EmptyEnvelope update_permission_async(tenant_id, security_permission_id, security_permission_update_dto, api_version, x_api_version)
Update an existing permission

Updates an existing security permission for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**security_permission_id** | **String** |  | [required] |
**security_permission_update_dto** | [**SecurityPermissionUpdateDto**](SecurityPermissionUpdateDto.md) |  | [required] |
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

