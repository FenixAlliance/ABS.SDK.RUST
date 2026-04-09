# \AccountGroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_account_group**](AccountGroupsApi.md#create_account_group) | **POST** /api/v2/AccountingService/AccountGroups | Creates a new account group
[**delete_account_group**](AccountGroupsApi.md#delete_account_group) | **DELETE** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Deletes an existing account group
[**get_account_group**](AccountGroupsApi.md#get_account_group) | **GET** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Gets the current tenant account group
[**get_account_groups**](AccountGroupsApi.md#get_account_groups) | **GET** /api/v2/AccountingService/AccountGroups | Gets the current tenant account groups
[**get_account_groups_count_async**](AccountGroupsApi.md#get_account_groups_count_async) | **GET** /api/v2/AccountingService/AccountGroups/Count | Gets the current tenant accounts count
[**update_account_group**](AccountGroupsApi.md#update_account_group) | **PUT** /api/v2/AccountingService/AccountGroups/{accountGroupId} | Updates an existing account group



## create_account_group

> models::AccountGroupDtoEnvelope create_account_group(tenant_id, api_version, x_api_version, account_group_create_dto)
Creates a new account group

Creates a new account group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_group_create_dto** | Option<[**AccountGroupCreateDto**](AccountGroupCreateDto.md)> |  |  |

### Return type

[**models::AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_account_group

> delete_account_group(tenant_id, account_group_id, api_version, x_api_version)
Deletes an existing account group

Deletes an existing account group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_group

> models::AccountGroupDtoEnvelope get_account_group(tenant_id, account_group_id, api_version, x_api_version)
Gets the current tenant account group

Get the currently acting tenant account group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_groups

> models::AccountGroupDtoListEnvelope get_account_groups(tenant_id, api_version, x_api_version)
Gets the current tenant account groups

Get the currently acting tenant account groups.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AccountGroupDtoListEnvelope**](AccountGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_groups_count_async

> models::Int32Envelope get_account_groups_count_async(tenant_id, api_version, x_api_version)
Gets the current tenant accounts count

Get the currently acting tenant accounts count.

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


## update_account_group

> models::AccountGroupDtoEnvelope update_account_group(tenant_id, account_group_id, api_version, x_api_version, account_group_update_dto)
Updates an existing account group

Updates an existing account group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**account_group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**account_group_update_dto** | Option<[**AccountGroupUpdateDto**](AccountGroupUpdateDto.md)> |  |  |

### Return type

[**models::AccountGroupDtoEnvelope**](AccountGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

