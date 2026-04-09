# \SyncApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sync_current_holder_to_current_tenant_crm**](SyncApi.md#sync_current_holder_to_current_tenant_crm) | **POST** /api/v2/CrmService/Sync | Sync the current user into the current tenant's contact list
[**sync_current_holder_to_tenant_crm**](SyncApi.md#sync_current_holder_to_tenant_crm) | **POST** /api/v2/CrmService/Sync/Me | Sync the current user into a tenant's contact list
[**sync_holder_to_tenant_crm_async**](SyncApi.md#sync_holder_to_tenant_crm_async) | **POST** /api/v2/CrmService/Sync/User | Sync a user into a tenant's contact list
[**sync_tenant_to_tenant_crm**](SyncApi.md#sync_tenant_to_tenant_crm) | **POST** /api/v2/CrmService/Sync/Tenant | Sync a tenant into another tenant's contact list



## sync_current_holder_to_current_tenant_crm

> models::Envelope sync_current_holder_to_current_tenant_crm(tenant_id, api_version, x_api_version)
Sync the current user into the current tenant's contact list

Synchronizes the currently authenticated user into the current tenant's CRM contact list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## sync_current_holder_to_tenant_crm

> models::Envelope sync_current_holder_to_tenant_crm(tenant_id, api_version, x_api_version)
Sync the current user into a tenant's contact list

Synchronizes the currently authenticated user into the specified tenant's CRM contact list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## sync_holder_to_tenant_crm_async

> models::Envelope sync_holder_to_tenant_crm_async(tenant_id, related_user_id, api_version, x_api_version)
Sync a user into a tenant's contact list

Synchronizes a specified user into the tenant's CRM contact list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**related_user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## sync_tenant_to_tenant_crm

> models::EmptyEnvelope sync_tenant_to_tenant_crm(tenant_id, related_tenant_id, api_version, x_api_version)
Sync a tenant into another tenant's contact list

Synchronizes a tenant into another tenant's CRM contact list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**related_tenant_id** | **uuid::Uuid** |  | [required] |
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

