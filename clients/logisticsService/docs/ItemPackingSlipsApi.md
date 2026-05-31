# \ItemPackingSlipsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_packing_slip_async**](ItemPackingSlipsApi.md#create_item_packing_slip_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips | Create an item packing slip
[**create_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#create_item_packing_slip_entry_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Create a packing slip entry
[**delete_item_packing_slip_async**](ItemPackingSlipsApi.md#delete_item_packing_slip_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Delete an item packing slip
[**delete_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#delete_item_packing_slip_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Delete a packing slip entry
[**get_item_packing_slip_by_id_async**](ItemPackingSlipsApi.md#get_item_packing_slip_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Get item packing slip by ID
[**get_item_packing_slip_entries_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entries_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Get packing slip entries
[**get_item_packing_slip_entries_count_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/Count | Get packing slip entries count
[**get_item_packing_slip_entry_by_id_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Get packing slip entry by ID
[**get_item_packing_slips_async**](ItemPackingSlipsApi.md#get_item_packing_slips_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips | Get all item packing slips
[**get_item_packing_slips_count_async**](ItemPackingSlipsApi.md#get_item_packing_slips_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/Count | Get item packing slips count
[**update_item_packing_slip_async**](ItemPackingSlipsApi.md#update_item_packing_slip_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Update an item packing slip
[**update_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#update_item_packing_slip_entry_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Update a packing slip entry



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

