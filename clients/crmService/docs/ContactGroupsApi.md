# \ContactGroupsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_group_async**](ContactGroupsApi.md#create_contact_group_async) | **POST** /api/v2/CrmService/ContactGroups | Create a new contact group
[**delete_contact_group_async**](ContactGroupsApi.md#delete_contact_group_async) | **DELETE** /api/v2/CrmService/ContactGroups/{id} | Delete a contact group
[**get_contact_group_by_id_async**](ContactGroupsApi.md#get_contact_group_by_id_async) | **GET** /api/v2/CrmService/ContactGroups/{id} | Get contact group by ID
[**get_contact_groups_async**](ContactGroupsApi.md#get_contact_groups_async) | **GET** /api/v2/CrmService/ContactGroups | Get all contact groups
[**get_contact_groups_count_async**](ContactGroupsApi.md#get_contact_groups_count_async) | **GET** /api/v2/CrmService/ContactGroups/Count | Get contact groups count
[**patch_contact_group_async**](ContactGroupsApi.md#patch_contact_group_async) | **PATCH** /api/v2/CrmService/ContactGroups/{id} | Patch a contact group
[**update_contact_group_async**](ContactGroupsApi.md#update_contact_group_async) | **PUT** /api/v2/CrmService/ContactGroups/{id} | Update a contact group



## create_contact_group_async

> create_contact_group_async(tenant_id, api_version, x_api_version, contacts_group_create_dto)
Create a new contact group

Creates a new contact group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contacts_group_create_dto** | Option<[**ContactsGroupCreateDto**](ContactsGroupCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_group_async

> delete_contact_group_async(tenant_id, id, api_version, x_api_version)
Delete a contact group

Deletes a contact group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_contact_group_by_id_async

> models::ContactsGroupDto get_contact_group_by_id_async(tenant_id, id, api_version, x_api_version)
Get contact group by ID

Retrieves a specific contact group by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactsGroupDto**](ContactsGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_groups_async

> models::ContactsGroupDtoListEnvelope get_contact_groups_async(tenant_id, api_version, x_api_version, contacts_group_dto_collection_query_parameters)
Get all contact groups

Retrieves all contact groups for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contacts_group_dto_collection_query_parameters** | Option<[**ContactsGroupDtoCollectionQueryParameters**](ContactsGroupDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ContactsGroupDtoListEnvelope**](ContactsGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_groups_count_async

> models::Int32Envelope get_contact_groups_count_async(tenant_id, api_version, x_api_version, contacts_group_dto_collection_query_parameters)
Get contact groups count

Returns the count of contact groups for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contacts_group_dto_collection_query_parameters** | Option<[**ContactsGroupDtoCollectionQueryParameters**](ContactsGroupDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_contact_group_async

> models::EmptyEnvelope patch_contact_group_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a contact group

Patch a contact group

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_contact_group_async

> update_contact_group_async(tenant_id, id, api_version, x_api_version, contacts_group_update_dto)
Update a contact group

Updates an existing contact group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contacts_group_update_dto** | Option<[**ContactsGroupUpdateDto**](ContactsGroupUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

