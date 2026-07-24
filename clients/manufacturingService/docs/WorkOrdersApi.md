# \WorkOrdersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_work_order_async**](WorkOrdersApi.md#create_work_order_async) | **POST** /api/v2/ManufacturingService/WorkOrders | Create a new work order
[**delete_work_order_async**](WorkOrdersApi.md#delete_work_order_async) | **DELETE** /api/v2/ManufacturingService/WorkOrders/{id} | Delete a work order
[**get_work_order_by_id_async**](WorkOrdersApi.md#get_work_order_by_id_async) | **GET** /api/v2/ManufacturingService/WorkOrders/{id} | Get work order by ID
[**get_work_orders_async**](WorkOrdersApi.md#get_work_orders_async) | **GET** /api/v2/ManufacturingService/WorkOrders | Get all work orders
[**get_work_orders_count_async**](WorkOrdersApi.md#get_work_orders_count_async) | **GET** /api/v2/ManufacturingService/WorkOrders/Count | Get work orders count
[**patch_work_order_async**](WorkOrdersApi.md#patch_work_order_async) | **PATCH** /api/v2/ManufacturingService/WorkOrders/{id} | Patch a work order
[**update_work_order_async**](WorkOrdersApi.md#update_work_order_async) | **PUT** /api/v2/ManufacturingService/WorkOrders/{id} | Update a work order



## create_work_order_async

> create_work_order_async(tenant_id, api_version, x_api_version, work_order_create_dto)
Create a new work order

Creates a new work order for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**work_order_create_dto** | Option<[**WorkOrderCreateDto**](WorkOrderCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_work_order_async

> delete_work_order_async(tenant_id, id, api_version, x_api_version)
Delete a work order

Deletes a work order for the specified tenant.

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


## get_work_order_by_id_async

> models::WorkOrderDto get_work_order_by_id_async(tenant_id, id, api_version, x_api_version)
Get work order by ID

Retrieves a specific work order by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkOrderDto**](WorkOrderDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_work_orders_async

> models::WorkOrderDtoListEnvelope get_work_orders_async(tenant_id, api_version, x_api_version)
Get all work orders

Retrieves all work orders for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkOrderDtoListEnvelope**](WorkOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_work_orders_count_async

> models::Int32Envelope get_work_orders_count_async(tenant_id, api_version, x_api_version)
Get work orders count

Returns the count of work orders for the specified tenant.

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


## patch_work_order_async

> models::EmptyEnvelope patch_work_order_async(tenant_id, id, api_version, x_api_version, operation)
Patch a work order

Patch a work order

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_work_order_async

> update_work_order_async(tenant_id, id, api_version, x_api_version, work_order_update_dto)
Update a work order

Updates an existing work order for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**work_order_update_dto** | Option<[**WorkOrderUpdateDto**](WorkOrderUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

