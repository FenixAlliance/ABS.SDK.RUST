# \ItemPickListsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_pick_list_async**](ItemPickListsApi.md#create_item_pick_list_async) | **POST** /api/v2/LogisticsService/ItemPickLists | Create an item pick list
[**create_item_pick_list_entry_async**](ItemPickListsApi.md#create_item_pick_list_entry_async) | **POST** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Create a pick list entry
[**delete_item_pick_list_async**](ItemPickListsApi.md#delete_item_pick_list_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Delete an item pick list
[**delete_item_pick_list_entry_async**](ItemPickListsApi.md#delete_item_pick_list_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Delete a pick list entry
[**get_item_pick_list_by_id_async**](ItemPickListsApi.md#get_item_pick_list_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Get item pick list by ID
[**get_item_pick_list_entries_async**](ItemPickListsApi.md#get_item_pick_list_entries_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Get pick list entries
[**get_item_pick_list_entries_count_async**](ItemPickListsApi.md#get_item_pick_list_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/Count | Get pick list entries count
[**get_item_pick_list_entry_by_id_async**](ItemPickListsApi.md#get_item_pick_list_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Get pick list entry by ID
[**get_item_pick_lists_async**](ItemPickListsApi.md#get_item_pick_lists_async) | **GET** /api/v2/LogisticsService/ItemPickLists | Get all item pick lists
[**get_item_pick_lists_count_async**](ItemPickListsApi.md#get_item_pick_lists_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/Count | Get item pick lists count
[**update_item_pick_list_async**](ItemPickListsApi.md#update_item_pick_list_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Update an item pick list
[**update_item_pick_list_entry_async**](ItemPickListsApi.md#update_item_pick_list_entry_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Update a pick list entry



## create_item_pick_list_async

> models::EmptyEnvelope create_item_pick_list_async(tenant_id, api_version, x_api_version, item_pick_list_create_dto)
Create an item pick list

Creates a new item pick list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_pick_list_create_dto** | Option<[**ItemPickListCreateDto**](ItemPickListCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_item_pick_list_entry_async

> models::EmptyEnvelope create_item_pick_list_entry_async(tenant_id, pick_list_id, api_version, x_api_version, item_pick_list_entry_create_dto)
Create a pick list entry

Creates a new pick list entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_pick_list_entry_create_dto** | Option<[**ItemPickListEntryCreateDto**](ItemPickListEntryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_pick_list_async

> models::EmptyEnvelope delete_item_pick_list_async(tenant_id, pick_list_id, api_version, x_api_version)
Delete an item pick list

Deletes an item pick list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
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


## delete_item_pick_list_entry_async

> models::EmptyEnvelope delete_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, api_version, x_api_version)
Delete a pick list entry

Deletes a pick list entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
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


## get_item_pick_list_by_id_async

> models::ItemPickListDtoEnvelope get_item_pick_list_by_id_async(tenant_id, pick_list_id, api_version, x_api_version)
Get item pick list by ID

Retrieves a specific item pick list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPickListDtoEnvelope**](ItemPickListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_pick_list_entries_async

> models::ItemPickListEntryDtoListEnvelope get_item_pick_list_entries_async(tenant_id, pick_list_id, api_version, x_api_version)
Get pick list entries

Retrieves all entries for the specified pick list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPickListEntryDtoListEnvelope**](ItemPickListEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_pick_list_entries_count_async

> models::Int32Envelope get_item_pick_list_entries_count_async(tenant_id, pick_list_id, api_version, x_api_version)
Get pick list entries count

Returns the count of pick list entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
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


## get_item_pick_list_entry_by_id_async

> models::ItemPickListEntryDtoEnvelope get_item_pick_list_entry_by_id_async(tenant_id, pick_list_id, entry_id, api_version, x_api_version)
Get pick list entry by ID

Retrieves a specific pick list entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPickListEntryDtoEnvelope**](ItemPickListEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_pick_lists_async

> models::ItemPickListDtoListEnvelope get_item_pick_lists_async(tenant_id, api_version, x_api_version)
Get all item pick lists

Retrieves all item pick lists for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPickListDtoListEnvelope**](ItemPickListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_pick_lists_count_async

> models::Int32Envelope get_item_pick_lists_count_async(tenant_id, api_version, x_api_version)
Get item pick lists count

Returns the count of item pick lists.

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


## update_item_pick_list_async

> models::EmptyEnvelope update_item_pick_list_async(tenant_id, pick_list_id, api_version, x_api_version, item_pick_list_update_dto)
Update an item pick list

Updates an existing item pick list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_pick_list_update_dto** | Option<[**ItemPickListUpdateDto**](ItemPickListUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_pick_list_entry_async

> models::EmptyEnvelope update_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, api_version, x_api_version, item_pick_list_entry_update_dto)
Update a pick list entry

Updates an existing pick list entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pick_list_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_pick_list_entry_update_dto** | Option<[**ItemPickListEntryUpdateDto**](ItemPickListEntryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

