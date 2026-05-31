# \WarehousesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_warehouse_async**](WarehousesApi.md#create_warehouse_async) | **POST** /api/v2/LogisticsService/Warehouses | Create a warehouse
[**delete_warehouse_async**](WarehousesApi.md#delete_warehouse_async) | **DELETE** /api/v2/LogisticsService/Warehouses/{warehouseId} | Delete a warehouse
[**get_warehouse_by_id_async**](WarehousesApi.md#get_warehouse_by_id_async) | **GET** /api/v2/LogisticsService/Warehouses/{warehouseId} | Get warehouse by ID
[**get_warehouses_async**](WarehousesApi.md#get_warehouses_async) | **GET** /api/v2/LogisticsService/Warehouses | Get all warehouses
[**get_warehouses_count_async**](WarehousesApi.md#get_warehouses_count_async) | **GET** /api/v2/LogisticsService/Warehouses/Count | Get warehouses count
[**update_warehouse_async**](WarehousesApi.md#update_warehouse_async) | **PUT** /api/v2/LogisticsService/Warehouses/{warehouseId} | Update a warehouse



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

