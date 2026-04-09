# \TenantsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**assign_license_async**](TenantsApi.md#assign_license_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Assign a license to a specific enrollment
[**create_tenant_async**](TenantsApi.md#create_tenant_async) | **POST** /api/v2/TenantsService/Tenants | Create a new business tenant
[**de_select_tenant_async**](TenantsApi.md#de_select_tenant_async) | **POST** /api/v2/TenantsService/Tenants/Deselect | Deselect the user's default tenant
[**delete_tenant_async**](TenantsApi.md#delete_tenant_async) | **DELETE** /api/v2/TenantsService/Tenants | Delete a tenant
[**get_accessible_features_async**](TenantsApi.md#get_accessible_features_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Features | Get the list of features accessible to a specific enrollment
[**get_current_tenant_async**](TenantsApi.md#get_current_tenant_async) | **GET** /api/v2/TenantsService/Tenants/Current | Get the user's current default tenant
[**get_enrollment_license_by_id_async**](TenantsApi.md#get_enrollment_license_by_id_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Get a specific license for an enrollment
[**get_enrollment_licenses_async**](TenantsApi.md#get_enrollment_licenses_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses | Get the list of licenses available to a specific enrollment
[**get_enrollment_permissions_async**](TenantsApi.md#get_enrollment_permissions_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Permissions | Get a specific tenant enrollment's permissions list
[**get_extended_tenant_async**](TenantsApi.md#get_extended_tenant_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Extended | Get an extended tenant's business profile
[**get_extended_tenant_enrollment_async**](TenantsApi.md#get_extended_tenant_enrollment_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Extended | Get a specific tenant enrollment
[**get_root_tenant_async**](TenantsApi.md#get_root_tenant_async) | **GET** /api/v2/TenantsService/Tenants/Root | Get the root tenant of the platform
[**get_tenant_async**](TenantsApi.md#get_tenant_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId} | Get a specific tenant by ID
[**get_tenant_avatar_async**](TenantsApi.md#get_tenant_avatar_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Avatar | Get a tenant's avatar
[**get_tenant_cart_async**](TenantsApi.md#get_tenant_cart_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Cart | Get a tenant's default cart
[**get_tenant_enrollment_async**](TenantsApi.md#get_tenant_enrollment_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId} | Get a specific tenant enrollment
[**get_tenant_enrollments_async**](TenantsApi.md#get_tenant_enrollments_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments | Get the list of user enrollments for a tenant
[**get_tenant_invitations_async**](TenantsApi.md#get_tenant_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations | Get the list of invitations issued by a tenant
[**get_tenant_licenses_async**](TenantsApi.md#get_tenant_licenses_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Licenses | Get the list of licenses available to a tenant
[**get_tenant_notifications_async**](TenantsApi.md#get_tenant_notifications_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Notifications | Get the list of notifications for a tenant
[**get_tenant_notifications_count_async**](TenantsApi.md#get_tenant_notifications_count_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Notifications/Count | Get the count of notifications for a tenant
[**get_tenant_pending_invitations_async**](TenantsApi.md#get_tenant_pending_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Pending | Get the list of invitations issued by a tenant that are pending
[**get_tenant_redeemed_invitations_async**](TenantsApi.md#get_tenant_redeemed_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Redeemed | Get the list of invitations issued by a tenant that have been redeemed
[**get_tenant_revoked_invitations_async**](TenantsApi.md#get_tenant_revoked_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Revoked | Get the list of invitations issued by a tenant that have been revoked
[**get_tenant_social_profile_async**](TenantsApi.md#get_tenant_social_profile_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/SocialProfile | Get a tenant's social profile
[**get_tenant_users_async**](TenantsApi.md#get_tenant_users_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Users | Get the list of users enrolled in a tenant
[**get_tenant_wallet_async**](TenantsApi.md#get_tenant_wallet_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Wallet | Get a tenant's billing profile (A.K.A. Wallet Account)
[**get_tenant_web_portals_async**](TenantsApi.md#get_tenant_web_portals_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/WebPortals | Get the list of web portals for a tenant
[**patch_tenant_async**](TenantsApi.md#patch_tenant_async) | **PATCH** /api/v2/TenantsService/Tenants/{tenantId} | Patch a tenant's profile
[**revoke_license_async**](TenantsApi.md#revoke_license_async) | **DELETE** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Revoke a license from a specific enrollment
[**select_tenant_async**](TenantsApi.md#select_tenant_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Select | Select a business tenant as the user's default tenant
[**update_avatar_async**](TenantsApi.md#update_avatar_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Avatar | Update a tenant's avatar
[**update_tenant_async**](TenantsApi.md#update_tenant_async) | **PUT** /api/v2/TenantsService/Tenants/{tenantId} | Update a tenant's profile
[**validate_enrollment_feature_access**](TenantsApi.md#validate_enrollment_feature_access) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/HasAccess | Validate the access to a specific feature for a specific enrollment
[**validate_enrollment_permissions_async**](TenantsApi.md#validate_enrollment_permissions_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Permissions/Validate | Validate the existence of a list of roles and permissions for a specific enrollment



## assign_license_async

> models::SuiteLicenseDtoListEnvelope assign_license_async(tenant_id, enrollment_id, license_id, api_version, x_api_version)
Assign a license to a specific enrollment

Assign a license to a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tenant_async

> models::EmptyEnvelope create_tenant_async(api_version, x_api_version, tenant_create_dto)
Create a new business tenant

Create a new business tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_create_dto** | Option<[**TenantCreateDto**](TenantCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## de_select_tenant_async

> models::EmptyEnvelope de_select_tenant_async(api_version, x_api_version)
Deselect the user's default tenant

Deselect the user's default tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## delete_tenant_async

> models::EmptyEnvelope delete_tenant_async(tenant_id, api_version, x_api_version)
Delete a tenant

Delete a business tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_accessible_features_async

> models::SuiteLicenseFeatureDtoListEnvelope get_accessible_features_async(tenant_id, enrollment_id, api_version, x_api_version)
Get the list of features accessible to a specific enrollment

Get the list of features accessible to a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseFeatureDtoListEnvelope**](SuiteLicenseFeatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_tenant_async

> models::TenantDtoEnvelope get_current_tenant_async(tenant_id, api_version, x_api_version)
Get the user's current default tenant

Get the user's current default tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollment_license_by_id_async

> models::SuiteLicenseDtoListEnvelope get_enrollment_license_by_id_async(tenant_id, enrollment_id, license_id, api_version, x_api_version)
Get a specific license for an enrollment

Get a specific license for an enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollment_licenses_async

> models::SuiteLicenseAssignmentDtoListEnvelope get_enrollment_licenses_async(tenant_id, enrollment_id, api_version, x_api_version)
Get the list of licenses available to a specific enrollment

Get the list of licenses available to a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseAssignmentDtoListEnvelope**](SuiteLicenseAssignmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollment_permissions_async

> models::StringListEnvelope get_enrollment_permissions_async(tenant_id, enrollment_id, api_version, x_api_version)
Get a specific tenant enrollment's permissions list

Get a specific tenant enrollment's permissions list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
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


## get_extended_tenant_async

> models::ExtendedTenantDtoEnvelope get_extended_tenant_async(tenant_id, api_version, x_api_version)
Get an extended tenant's business profile

Get an extended tenant's business profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedTenantDtoEnvelope**](ExtendedTenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_tenant_enrollment_async

> models::ExtendedTenantEnrollmentDtoEnvelope get_extended_tenant_enrollment_async(tenant_id, enrollment_id, api_version, x_api_version)
Get a specific tenant enrollment

Get a specific tenant enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedTenantEnrollmentDtoEnvelope**](ExtendedTenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_root_tenant_async

> models::TenantDtoEnvelope get_root_tenant_async(api_version, x_api_version)
Get the root tenant of the platform

Get the root tenant of the platform

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_async

> models::TenantDtoEnvelope get_tenant_async(tenant_id, api_version, x_api_version)
Get a specific tenant by ID

Get a specific tenant by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_avatar_async

> models::EmptyEnvelope get_tenant_avatar_async(tenant_id, api_version, x_api_version)
Get a tenant's avatar

Get a tenant's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_tenant_cart_async

> models::CartDtoEnvelope get_tenant_cart_async(tenant_id, api_version, x_api_version)
Get a tenant's default cart

Get a tenant's default cart

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_enrollment_async

> models::TenantEnrollmentDtoEnvelope get_tenant_enrollment_async(tenant_id, enrollment_id, api_version, x_api_version)
Get a specific tenant enrollment

Get a specific tenant enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantEnrollmentDtoEnvelope**](TenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_enrollments_async

> models::TenantEnrollmentDtoListEnvelope get_tenant_enrollments_async(tenant_id, api_version, x_api_version)
Get the list of user enrollments for a tenant

Get the list of user enrollments for a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_invitations_async

> models::TenantInvitationDtoListEnvelope get_tenant_invitations_async(tenant_id, api_version, x_api_version)
Get the list of invitations issued by a tenant

Get the list of invitations issued by a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_licenses_async

> models::SuiteLicenseDtoListEnvelope get_tenant_licenses_async(tenant_id, api_version, x_api_version)
Get the list of licenses available to a tenant

Get the list of licenses available to a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_notifications_async

> models::NotificationDtoListEnvelope get_tenant_notifications_async(tenant_id, api_version, x_api_version)
Get the list of notifications for a tenant

Get the list of notifications for a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NotificationDtoListEnvelope**](NotificationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_notifications_count_async

> models::Int32Envelope get_tenant_notifications_count_async(tenant_id, api_version, x_api_version)
Get the count of notifications for a tenant

Get the count of notifications for a tenant

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


## get_tenant_pending_invitations_async

> models::TenantInvitationDtoListEnvelope get_tenant_pending_invitations_async(tenant_id, api_version, x_api_version)
Get the list of invitations issued by a tenant that are pending

Get the list of invitations issued by a tenant that are pending

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_redeemed_invitations_async

> models::TenantInvitationDtoListEnvelope get_tenant_redeemed_invitations_async(tenant_id, api_version, x_api_version)
Get the list of invitations issued by a tenant that have been redeemed

Get the list of invitations issued by a tenant that have been redeemed

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_revoked_invitations_async

> models::TenantInvitationDtoListEnvelope get_tenant_revoked_invitations_async(tenant_id, api_version, x_api_version)
Get the list of invitations issued by a tenant that have been revoked

Get the list of invitations issued by a tenant that have been revoked

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_social_profile_async

> models::SocialProfileDtoEnvelope get_tenant_social_profile_async(tenant_id, api_version, x_api_version)
Get a tenant's social profile

Get a tenant's social profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_users_async

> models::UserDtoListEnvelope get_tenant_users_async(tenant_id, api_version, x_api_version)
Get the list of users enrolled in a tenant

Get the list of users enrolled in a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserDtoListEnvelope**](UserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_wallet_async

> models::WalletDtoEnvelope get_tenant_wallet_async(tenant_id, api_version, x_api_version)
Get a tenant's billing profile (A.K.A. Wallet Account)

Get a tenant's billing profile (A.K.A. Wallet Account)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_web_portals_async

> models::WebPortalDtoListEnvelope get_tenant_web_portals_async(tenant_id, api_version, x_api_version)
Get the list of web portals for a tenant

Get the list of web portals for a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoListEnvelope**](WebPortalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_tenant_async

> models::EmptyEnvelope patch_tenant_async(tenant_id, api_version, x_api_version, operation)
Patch a tenant's profile

Patch a tenant's profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## revoke_license_async

> models::SuiteLicenseDtoListEnvelope revoke_license_async(tenant_id, enrollment_id, license_id, api_version, x_api_version)
Revoke a license from a specific enrollment

Revoke a license from a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## select_tenant_async

> models::EmptyEnvelope select_tenant_async(tenant_id, api_version, x_api_version)
Select a business tenant as the user's default tenant

Select a business tenant as the user's default tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## update_avatar_async

> models::EmptyEnvelope update_avatar_async(tenant_id, api_version, x_api_version, avatar)
Update a tenant's avatar

Update a tenant's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**avatar** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: image/png, application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tenant_async

> models::EmptyEnvelope update_tenant_async(tenant_id, api_version, x_api_version, tenant_update_dto)
Update a tenant's profile

Update a tenant's profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_update_dto** | Option<[**TenantUpdateDto**](TenantUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## validate_enrollment_feature_access

> models::BooleanEnvelope validate_enrollment_feature_access(tenant_id, enrollment_id, feature, api_version, x_api_version)
Validate the access to a specific feature for a specific enrollment

Validate the access to a specific feature for a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**feature** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## validate_enrollment_permissions_async

> models::BooleanEnvelope validate_enrollment_permissions_async(tenant_id, enrollment_id, roles, permissions, api_version, x_api_version)
Validate the existence of a list of roles and permissions for a specific enrollment

Validate the existence of a list of roles and permissions for a specific enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**enrollment_id** | **uuid::Uuid** |  | [required] |
**roles** | Option<[**Vec<String>**](String.md)> |  |  |
**permissions** | Option<[**Vec<String>**](String.md)> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

