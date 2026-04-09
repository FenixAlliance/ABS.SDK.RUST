# \EmailGroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_email_group_async**](EmailGroupsApi.md#create_email_group_async) | **POST** /api/v2/MarketingService/EmailGroups | Create an email group
[**delete_email_group_async**](EmailGroupsApi.md#delete_email_group_async) | **DELETE** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Delete an email group
[**get_email_group_details_async**](EmailGroupsApi.md#get_email_group_details_async) | **GET** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Get email group by ID
[**get_email_groups_count_async**](EmailGroupsApi.md#get_email_groups_count_async) | **GET** /api/v2/MarketingService/EmailGroups/Count | Get email groups count
[**get_email_groups_o_data_async**](EmailGroupsApi.md#get_email_groups_o_data_async) | **GET** /api/v2/MarketingService/EmailGroups | Get email groups
[**update_email_group_async**](EmailGroupsApi.md#update_email_group_async) | **PUT** /api/v2/MarketingService/EmailGroups/{emailgroupId} | Update an email group



## create_email_group_async

> models::EmptyEnvelope create_email_group_async(tenant_id, email_group_create_dto, api_version, x_api_version)
Create an email group

Creates a new email group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_group_create_dto** | [**EmailGroupCreateDto**](EmailGroupCreateDto.md) |  | [required] |
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


## delete_email_group_async

> models::EmptyEnvelope delete_email_group_async(tenant_id, emailgroup_id, api_version, x_api_version)
Delete an email group

Deletes an email group by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailgroup_id** | **uuid::Uuid** |  | [required] |
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


## get_email_group_details_async

> models::EmailGroupDtoEnvelope get_email_group_details_async(tenant_id, emailgroup_id, api_version, x_api_version)
Get email group by ID

Retrieves the details of a specific email group by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailgroup_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailGroupDtoEnvelope**](EmailGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_email_groups_count_async

> models::Int32Envelope get_email_groups_count_async(tenant_id, api_version, x_api_version)
Get email groups count

Returns the count of email groups for the specified tenant using OData query options.

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


## get_email_groups_o_data_async

> models::EmailGroupDtoListEnvelope get_email_groups_o_data_async(tenant_id, api_version, x_api_version)
Get email groups

Retrieves a collection of email groups for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailGroupDtoListEnvelope**](EmailGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_email_group_async

> models::EmptyEnvelope update_email_group_async(tenant_id, emailgroup_id, email_group_update_dto, api_version, x_api_version)
Update an email group

Updates an existing email group by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailgroup_id** | **uuid::Uuid** |  | [required] |
**email_group_update_dto** | [**EmailGroupUpdateDto**](EmailGroupUpdateDto.md) |  | [required] |
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

