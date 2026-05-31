# \ItemRestocksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_restock_async**](ItemRestocksApi.md#create_item_restock_async) | **POST** /api/v2/LogisticsService/ItemRestocks | Create an item restock
[**create_item_restock_entry_async**](ItemRestocksApi.md#create_item_restock_entry_async) | **POST** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Create a restock entry
[**delete_item_restock_async**](ItemRestocksApi.md#delete_item_restock_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId} | Delete an item restock
[**delete_item_restock_entry_async**](ItemRestocksApi.md#delete_item_restock_entry_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Delete a restock entry
[**get_item_restock_by_id_async**](ItemRestocksApi.md#get_item_restock_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId} | Get item restock by ID
[**get_item_restock_entries_async**](ItemRestocksApi.md#get_item_restock_entries_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Get restock entries
[**get_item_restock_entries_count_async**](ItemRestocksApi.md#get_item_restock_entries_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/Count | Get restock entries count
[**get_item_restock_entry_by_id_async**](ItemRestocksApi.md#get_item_restock_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Get restock entry by ID
[**get_item_restocks_async**](ItemRestocksApi.md#get_item_restocks_async) | **GET** /api/v2/LogisticsService/ItemRestocks | Get all item restocks
[**get_item_restocks_count_async**](ItemRestocksApi.md#get_item_restocks_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/Count | Get item restocks count
[**update_item_restock_async**](ItemRestocksApi.md#update_item_restock_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId} | Update an item restock
[**update_item_restock_entry_async**](ItemRestocksApi.md#update_item_restock_entry_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Update a restock entry



## create_item_restock_async

> models::EmptyEnvelope create_item_restock_async(tenant_id, api_version, x_api_version, item_restock_create_dto)
Create an item restock

Creates a new item restock.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_restock_create_dto** | Option<[**ItemRestockCreateDto**](ItemRestockCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_item_restock_entry_async

> models::EmptyEnvelope create_item_restock_entry_async(tenant_id, restock_id, api_version, x_api_version, item_restock_entry_create_dto)
Create a restock entry

Creates a new restock entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_restock_entry_create_dto** | Option<[**ItemRestockEntryCreateDto**](ItemRestockEntryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_restock_async

> models::EmptyEnvelope delete_item_restock_async(tenant_id, restock_id, api_version, x_api_version)
Delete an item restock

Deletes an item restock.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
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


## delete_item_restock_entry_async

> models::EmptyEnvelope delete_item_restock_entry_async(tenant_id, restock_id, entry_id, api_version, x_api_version)
Delete a restock entry

Deletes a restock entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
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


## get_item_restock_by_id_async

> models::ItemRestockDtoEnvelope get_item_restock_by_id_async(tenant_id, restock_id, api_version, x_api_version)
Get item restock by ID

Retrieves a specific item restock.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRestockDtoEnvelope**](ItemRestockDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_restock_entries_async

> models::ItemRestockEntryDtoListEnvelope get_item_restock_entries_async(tenant_id, restock_id, api_version, x_api_version)
Get restock entries

Retrieves all entries for the specified restock.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRestockEntryDtoListEnvelope**](ItemRestockEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_restock_entries_count_async

> models::Int32Envelope get_item_restock_entries_count_async(tenant_id, restock_id, api_version, x_api_version)
Get restock entries count

Returns the count of restock entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
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


## get_item_restock_entry_by_id_async

> models::ItemRestockEntryDtoEnvelope get_item_restock_entry_by_id_async(tenant_id, restock_id, entry_id, api_version, x_api_version)
Get restock entry by ID

Retrieves a specific restock entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRestockEntryDtoEnvelope**](ItemRestockEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_restocks_async

> models::ItemRestockDtoListEnvelope get_item_restocks_async(tenant_id, api_version, x_api_version)
Get all item restocks

Retrieves all item restocks for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRestockDtoListEnvelope**](ItemRestockDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_restocks_count_async

> models::Int32Envelope get_item_restocks_count_async(tenant_id, api_version, x_api_version)
Get item restocks count

Returns the count of item restocks.

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


## update_item_restock_async

> models::EmptyEnvelope update_item_restock_async(tenant_id, restock_id, api_version, x_api_version, item_restock_update_dto)
Update an item restock

Updates an existing item restock.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_restock_update_dto** | Option<[**ItemRestockUpdateDto**](ItemRestockUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_restock_entry_async

> models::EmptyEnvelope update_item_restock_entry_async(tenant_id, restock_id, entry_id, api_version, x_api_version, item_restock_entry_update_dto)
Update a restock entry

Updates an existing restock entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**restock_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_restock_entry_update_dto** | Option<[**ItemRestockEntryUpdateDto**](ItemRestockEntryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

