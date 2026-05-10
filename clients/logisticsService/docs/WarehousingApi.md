# \WarehousingApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_packing_slip_async**](WarehousingApi.md#create_item_packing_slip_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips | Create an item packing slip
[**create_item_packing_slip_entry_async**](WarehousingApi.md#create_item_packing_slip_entry_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Create a packing slip entry
[**create_item_pick_list_async**](WarehousingApi.md#create_item_pick_list_async) | **POST** /api/v2/LogisticsService/ItemPickLists | Create an item pick list
[**create_item_pick_list_entry_async**](WarehousingApi.md#create_item_pick_list_entry_async) | **POST** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Create a pick list entry
[**create_item_restock_async**](WarehousingApi.md#create_item_restock_async) | **POST** /api/v2/LogisticsService/ItemRestocks | Create an item restock
[**create_item_restock_entry_async**](WarehousingApi.md#create_item_restock_entry_async) | **POST** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Create a restock entry
[**create_item_retain_sample_async**](WarehousingApi.md#create_item_retain_sample_async) | **POST** /api/v2/LogisticsService/ItemRetainSamples | Create an item retain sample
[**create_warehouse_async**](WarehousingApi.md#create_warehouse_async) | **POST** /api/v2/LogisticsService/Warehouses | Create a warehouse
[**delete_item_packing_slip_async**](WarehousingApi.md#delete_item_packing_slip_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Delete an item packing slip
[**delete_item_packing_slip_entry_async**](WarehousingApi.md#delete_item_packing_slip_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Delete a packing slip entry
[**delete_item_pick_list_async**](WarehousingApi.md#delete_item_pick_list_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Delete an item pick list
[**delete_item_pick_list_entry_async**](WarehousingApi.md#delete_item_pick_list_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Delete a pick list entry
[**delete_item_restock_async**](WarehousingApi.md#delete_item_restock_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId} | Delete an item restock
[**delete_item_restock_entry_async**](WarehousingApi.md#delete_item_restock_entry_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Delete a restock entry
[**delete_item_retain_sample_async**](WarehousingApi.md#delete_item_retain_sample_async) | **DELETE** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Delete an item retain sample
[**delete_warehouse_async**](WarehousingApi.md#delete_warehouse_async) | **DELETE** /api/v2/LogisticsService/Warehouses/{warehouseId} | Delete a warehouse
[**get_item_packing_slip_by_id_async**](WarehousingApi.md#get_item_packing_slip_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Get item packing slip by ID
[**get_item_packing_slip_entries_async**](WarehousingApi.md#get_item_packing_slip_entries_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Get packing slip entries
[**get_item_packing_slip_entries_count_async**](WarehousingApi.md#get_item_packing_slip_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/Count | Get packing slip entries count
[**get_item_packing_slip_entry_by_id_async**](WarehousingApi.md#get_item_packing_slip_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Get packing slip entry by ID
[**get_item_packing_slips_async**](WarehousingApi.md#get_item_packing_slips_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips | Get all item packing slips
[**get_item_packing_slips_count_async**](WarehousingApi.md#get_item_packing_slips_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/Count | Get item packing slips count
[**get_item_pick_list_by_id_async**](WarehousingApi.md#get_item_pick_list_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Get item pick list by ID
[**get_item_pick_list_entries_async**](WarehousingApi.md#get_item_pick_list_entries_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Get pick list entries
[**get_item_pick_list_entries_count_async**](WarehousingApi.md#get_item_pick_list_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/Count | Get pick list entries count
[**get_item_pick_list_entry_by_id_async**](WarehousingApi.md#get_item_pick_list_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Get pick list entry by ID
[**get_item_pick_lists_async**](WarehousingApi.md#get_item_pick_lists_async) | **GET** /api/v2/LogisticsService/ItemPickLists | Get all item pick lists
[**get_item_pick_lists_count_async**](WarehousingApi.md#get_item_pick_lists_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/Count | Get item pick lists count
[**get_item_restock_by_id_async**](WarehousingApi.md#get_item_restock_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId} | Get item restock by ID
[**get_item_restock_entries_async**](WarehousingApi.md#get_item_restock_entries_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Get restock entries
[**get_item_restock_entries_count_async**](WarehousingApi.md#get_item_restock_entries_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/Count | Get restock entries count
[**get_item_restock_entry_by_id_async**](WarehousingApi.md#get_item_restock_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Get restock entry by ID
[**get_item_restocks_async**](WarehousingApi.md#get_item_restocks_async) | **GET** /api/v2/LogisticsService/ItemRestocks | Get all item restocks
[**get_item_restocks_count_async**](WarehousingApi.md#get_item_restocks_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/Count | Get item restocks count
[**get_item_retain_sample_by_id_async**](WarehousingApi.md#get_item_retain_sample_by_id_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Get item retain sample by ID
[**get_item_retain_samples_async**](WarehousingApi.md#get_item_retain_samples_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples | Get all item retain samples
[**get_item_retain_samples_count_async**](WarehousingApi.md#get_item_retain_samples_count_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/Count | Get item retain samples count
[**get_warehouse_by_id_async**](WarehousingApi.md#get_warehouse_by_id_async) | **GET** /api/v2/LogisticsService/Warehouses/{warehouseId} | Get warehouse by ID
[**get_warehouses_async**](WarehousingApi.md#get_warehouses_async) | **GET** /api/v2/LogisticsService/Warehouses | Get all warehouses
[**get_warehouses_count_async**](WarehousingApi.md#get_warehouses_count_async) | **GET** /api/v2/LogisticsService/Warehouses/Count | Get warehouses count
[**update_item_packing_slip_async**](WarehousingApi.md#update_item_packing_slip_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Update an item packing slip
[**update_item_packing_slip_entry_async**](WarehousingApi.md#update_item_packing_slip_entry_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Update a packing slip entry
[**update_item_pick_list_async**](WarehousingApi.md#update_item_pick_list_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Update an item pick list
[**update_item_pick_list_entry_async**](WarehousingApi.md#update_item_pick_list_entry_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Update a pick list entry
[**update_item_restock_async**](WarehousingApi.md#update_item_restock_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId} | Update an item restock
[**update_item_restock_entry_async**](WarehousingApi.md#update_item_restock_entry_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Update a restock entry
[**update_item_retain_sample_async**](WarehousingApi.md#update_item_retain_sample_async) | **PUT** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Update an item retain sample
[**update_warehouse_async**](WarehousingApi.md#update_warehouse_async) | **PUT** /api/v2/LogisticsService/Warehouses/{warehouseId} | Update a warehouse



## create_item_packing_slip_async

> models::EmptyEnvelope create_item_packing_slip_async(tenant_id, api_version, x_api_version, item_packing_slip_create_dto)
Create an item packing slip

Creates a new item packing slip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_packing_slip_create_dto** | Option<[**ItemPackingSlipCreateDto**](ItemPackingSlipCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_item_packing_slip_entry_async

> models::EmptyEnvelope create_item_packing_slip_entry_async(tenant_id, packing_slip_id, api_version, x_api_version, item_packing_slip_entry_create_dto)
Create a packing slip entry

Creates a new packing slip entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_packing_slip_entry_create_dto** | Option<[**ItemPackingSlipEntryCreateDto**](ItemPackingSlipEntryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


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


## create_item_retain_sample_async

> models::EmptyEnvelope create_item_retain_sample_async(tenant_id, api_version, x_api_version, item_retain_sample_create_dto)
Create an item retain sample

Creates a new item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_retain_sample_create_dto** | Option<[**ItemRetainSampleCreateDto**](ItemRetainSampleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_warehouse_async

> models::EmptyEnvelope create_warehouse_async(tenant_id, api_version, x_api_version, warehouse_create_dto)
Create a warehouse

Creates a new warehouse.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**warehouse_create_dto** | Option<[**WarehouseCreateDto**](WarehouseCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_packing_slip_async

> models::EmptyEnvelope delete_item_packing_slip_async(tenant_id, packing_slip_id, api_version, x_api_version)
Delete an item packing slip

Deletes an item packing slip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
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


## delete_item_packing_slip_entry_async

> models::EmptyEnvelope delete_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, api_version, x_api_version)
Delete a packing slip entry

Deletes a packing slip entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
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


## delete_item_retain_sample_async

> models::EmptyEnvelope delete_item_retain_sample_async(tenant_id, retain_sample_id, api_version, x_api_version)
Delete an item retain sample

Deletes an item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
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


## delete_warehouse_async

> models::EmptyEnvelope delete_warehouse_async(tenant_id, warehouse_id, api_version, x_api_version)
Delete a warehouse

Deletes a warehouse.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warehouse_id** | **uuid::Uuid** |  | [required] |
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


## get_item_packing_slip_by_id_async

> models::ItemPackingSlipDtoEnvelope get_item_packing_slip_by_id_async(tenant_id, packing_slip_id, api_version, x_api_version)
Get item packing slip by ID

Retrieves a specific item packing slip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPackingSlipDtoEnvelope**](ItemPackingSlipDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_packing_slip_entries_async

> models::ItemPackingSlipEntryDtoListEnvelope get_item_packing_slip_entries_async(tenant_id, packing_slip_id, api_version, x_api_version)
Get packing slip entries

Retrieves all entries for the specified packing slip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPackingSlipEntryDtoListEnvelope**](ItemPackingSlipEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_packing_slip_entries_count_async

> models::Int32Envelope get_item_packing_slip_entries_count_async(tenant_id, packing_slip_id, api_version, x_api_version)
Get packing slip entries count

Returns the count of packing slip entries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
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


## get_item_packing_slip_entry_by_id_async

> models::ItemPackingSlipEntryDtoEnvelope get_item_packing_slip_entry_by_id_async(tenant_id, packing_slip_id, entry_id, api_version, x_api_version)
Get packing slip entry by ID

Retrieves a specific packing slip entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPackingSlipEntryDtoEnvelope**](ItemPackingSlipEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_packing_slips_async

> models::ItemPackingSlipDtoListEnvelope get_item_packing_slips_async(tenant_id, api_version, x_api_version)
Get all item packing slips

Retrieves all item packing slips for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemPackingSlipDtoListEnvelope**](ItemPackingSlipDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_packing_slips_count_async

> models::Int32Envelope get_item_packing_slips_count_async(tenant_id, api_version, x_api_version)
Get item packing slips count

Returns the count of item packing slips.

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


## get_item_retain_sample_by_id_async

> models::ItemRetainSampleDtoEnvelope get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, api_version, x_api_version)
Get item retain sample by ID

Retrieves a specific item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRetainSampleDtoEnvelope**](ItemRetainSampleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_retain_samples_async

> models::ItemRetainSampleDtoListEnvelope get_item_retain_samples_async(tenant_id, api_version, x_api_version)
Get all item retain samples

Retrieves all item retain samples for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRetainSampleDtoListEnvelope**](ItemRetainSampleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_retain_samples_count_async

> models::Int32Envelope get_item_retain_samples_count_async(tenant_id, api_version, x_api_version)
Get item retain samples count

Returns the count of item retain samples.

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


## get_warehouse_by_id_async

> models::WarehouseDtoEnvelope get_warehouse_by_id_async(tenant_id, warehouse_id, api_version, x_api_version)
Get warehouse by ID

Retrieves a specific warehouse.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warehouse_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WarehouseDtoEnvelope**](WarehouseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_warehouses_async

> models::WarehouseDtoListEnvelope get_warehouses_async(tenant_id, api_version, x_api_version)
Get all warehouses

Retrieves all warehouses for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WarehouseDtoListEnvelope**](WarehouseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_warehouses_count_async

> models::Int32Envelope get_warehouses_count_async(tenant_id, api_version, x_api_version)
Get warehouses count

Returns the count of warehouses.

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


## update_item_packing_slip_async

> models::EmptyEnvelope update_item_packing_slip_async(tenant_id, packing_slip_id, api_version, x_api_version, item_packing_slip_update_dto)
Update an item packing slip

Updates an existing item packing slip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_packing_slip_update_dto** | Option<[**ItemPackingSlipUpdateDto**](ItemPackingSlipUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_packing_slip_entry_async

> models::EmptyEnvelope update_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, api_version, x_api_version, item_packing_slip_entry_update_dto)
Update a packing slip entry

Updates an existing packing slip entry.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**packing_slip_id** | **uuid::Uuid** |  | [required] |
**entry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_packing_slip_entry_update_dto** | Option<[**ItemPackingSlipEntryUpdateDto**](ItemPackingSlipEntryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
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


## update_item_retain_sample_async

> models::EmptyEnvelope update_item_retain_sample_async(tenant_id, retain_sample_id, api_version, x_api_version, item_retain_sample_update_dto)
Update an item retain sample

Updates an existing item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_retain_sample_update_dto** | Option<[**ItemRetainSampleUpdateDto**](ItemRetainSampleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_warehouse_async

> models::EmptyEnvelope update_warehouse_async(tenant_id, warehouse_id, api_version, x_api_version, warehouse_update_dto)
Update a warehouse

Updates an existing warehouse.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**warehouse_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**warehouse_update_dto** | Option<[**WarehouseUpdateDto**](WarehouseUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

