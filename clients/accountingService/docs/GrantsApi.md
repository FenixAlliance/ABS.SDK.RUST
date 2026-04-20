# \GrantsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_grant_async**](GrantsApi.md#create_grant_async) | **POST** /api/v2/AccountingService/Grants | Create grant
[**delete_grant_async**](GrantsApi.md#delete_grant_async) | **DELETE** /api/v2/AccountingService/Grants/{grantId} | Delete grant
[**get_grant_details_async**](GrantsApi.md#get_grant_details_async) | **GET** /api/v2/AccountingService/Grants/{grantId} | Get grant by ID
[**get_grants_async**](GrantsApi.md#get_grants_async) | **GET** /api/v2/AccountingService/Grants | Get all grants
[**get_grants_count_async**](GrantsApi.md#get_grants_count_async) | **GET** /api/v2/AccountingService/Grants/Count | Count grants
[**update_grant_async**](GrantsApi.md#update_grant_async) | **PUT** /api/v2/AccountingService/Grants/{grantId} | Update grant



## create_grant_async

> models::EmptyEnvelope create_grant_async(tenant_id, api_version, x_api_version, grant_create_dto)
Create grant

Creates a new grant entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**grant_create_dto** | Option<[**GrantCreateDto**](GrantCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_grant_async

> models::EmptyEnvelope delete_grant_async(tenant_id, grant_id, api_version, x_api_version)
Delete grant

Deletes a grant identified by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**grant_id** | **uuid::Uuid** |  | [required] |
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


## get_grant_details_async

> models::GrantDtoEnvelope get_grant_details_async(tenant_id, grant_id, api_version, x_api_version)
Get grant by ID

Gets detailed information for a specific grant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**grant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GrantDtoEnvelope**](GrantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_grants_async

> models::GrantDtoIReadOnlyListEnvelope get_grants_async(tenant_id, api_version, x_api_version)
Get all grants

Retrieves a list of grants associated with the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GrantDtoIReadOnlyListEnvelope**](GrantDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_grants_count_async

> models::Int32Envelope get_grants_count_async(tenant_id, api_version, x_api_version)
Count grants

Returns the number of grants for the tenant.

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


## update_grant_async

> models::EmptyEnvelope update_grant_async(tenant_id, grant_id, api_version, x_api_version, body)
Update grant

Updates an existing grant identified by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**grant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**body** | Option<**serde_json::Value**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

