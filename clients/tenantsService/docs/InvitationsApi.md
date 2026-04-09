# \InvitationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accept_tenant_invitation**](InvitationsApi.md#accept_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations/{invitationId}/Accept | Accept an invitation to join a tenant
[**decline_tenant_invitation**](InvitationsApi.md#decline_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations/{invitationId}/Decline | Decline an invitation to join a tenant
[**delete_tenant_invitation**](InvitationsApi.md#delete_tenant_invitation) | **DELETE** /api/v2/TenantsService/Invitations/{invitationId} | Delete a tenant invitation
[**get_tenant_invitation_by_id**](InvitationsApi.md#get_tenant_invitation_by_id) | **GET** /api/v2/TenantsService/Invitations/{invitationId} | Get a tenant invitation by its ID
[**get_tenant_invitations**](InvitationsApi.md#get_tenant_invitations) | **GET** /api/v2/TenantsService/Invitations | Retrieve a list of tenant invitations
[**get_tenant_invitations_count**](InvitationsApi.md#get_tenant_invitations_count) | **GET** /api/v2/TenantsService/Invitations/Count | Get the count of tenant invitations
[**send_tenant_invitation**](InvitationsApi.md#send_tenant_invitation) | **POST** /api/v2/TenantsService/Invitations | Send an invitation to a user to join a tenant



## accept_tenant_invitation

> models::EmptyEnvelope accept_tenant_invitation(invitation_id, api_version, x_api_version)
Accept an invitation to join a tenant

Accept an invitation to join a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invitation_id** | **uuid::Uuid** |  | [required] |
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


## decline_tenant_invitation

> models::EmptyEnvelope decline_tenant_invitation(invitation_id, api_version, x_api_version)
Decline an invitation to join a tenant

Decline an invitation to join a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invitation_id** | **uuid::Uuid** |  | [required] |
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


## delete_tenant_invitation

> models::EmptyEnvelope delete_tenant_invitation(tenant_id, invitation_id, api_version, x_api_version)
Delete a tenant invitation

Delete a tenant invitation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invitation_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_invitation_by_id

> models::TenantInvitationDtoEnvelope get_tenant_invitation_by_id(tenant_id, invitation_id, api_version, x_api_version)
Get a tenant invitation by its ID

Get a tenant invitation by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invitation_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoEnvelope**](TenantInvitationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_invitations

> models::TenantInvitationDtoListEnvelope get_tenant_invitations(tenant_id, api_version, x_api_version)
Retrieve a list of tenant invitations

Retrieve a list of tenant invitations

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


## get_tenant_invitations_count

> models::Int32Envelope get_tenant_invitations_count(tenant_id, api_version, x_api_version)
Get the count of tenant invitations

Get the count of tenant invitations

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


## send_tenant_invitation

> models::EmptyEnvelope send_tenant_invitation(tenant_id, api_version, x_api_version, tenant_invitation_create_dto)
Send an invitation to a user to join a tenant

Send an invitation to a user to join a tenant

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_invitation_create_dto** | Option<[**TenantInvitationCreateDto**](TenantInvitationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

