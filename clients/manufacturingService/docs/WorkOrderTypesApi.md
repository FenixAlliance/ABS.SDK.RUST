# \WorkOrderTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_work_order_type_async**](WorkOrderTypesApi.md#create_work_order_type_async) | **POST** /api/v2/ManufacturingService/WorkOrderTypes | Create a new work order type
[**delete_work_order_type_async**](WorkOrderTypesApi.md#delete_work_order_type_async) | **DELETE** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Delete a work order type
[**get_work_order_type_by_id_async**](WorkOrderTypesApi.md#get_work_order_type_by_id_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Get work order type by ID
[**get_work_order_types_async**](WorkOrderTypesApi.md#get_work_order_types_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes | Get all work order types
[**get_work_order_types_count_async**](WorkOrderTypesApi.md#get_work_order_types_count_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes/Count | Get work order types count
[**patch_work_order_type_async**](WorkOrderTypesApi.md#patch_work_order_type_async) | **PATCH** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Patch a work order type
[**update_work_order_type_async**](WorkOrderTypesApi.md#update_work_order_type_async) | **PUT** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Update a work order type



## create_work_order_type_async

> create_work_order_type_async(tenant_id, api_version, x_api_version, work_order_type_create_dto)
Create a new work order type

Creates a new work order type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**work_order_type_create_dto** | Option<[**WorkOrderTypeCreateDto**](WorkOrderTypeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_work_order_type_async

> delete_work_order_type_async(tenant_id, id, api_version, x_api_version)
Delete a work order type

Deletes a work order type for the specified tenant.

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


## get_work_order_type_by_id_async

> models::WorkOrderTypeDto get_work_order_type_by_id_async(tenant_id, id, api_version, x_api_version)
Get work order type by ID

Retrieves a specific work order type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkOrderTypeDto**](WorkOrderTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_work_order_types_async

> models::WorkOrderTypeDtoListEnvelope get_work_order_types_async(tenant_id, api_version, x_api_version)
Get all work order types

Retrieves all work order types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkOrderTypeDtoListEnvelope**](WorkOrderTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_work_order_types_count_async

> models::Int32Envelope get_work_order_types_count_async(tenant_id, api_version, x_api_version)
Get work order types count

Returns the count of work order types for the specified tenant.

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


## patch_work_order_type_async

> models::EmptyEnvelope patch_work_order_type_async(tenant_id, id, api_version, x_api_version, operation)
Patch a work order type

Patch a work order type

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


## update_work_order_type_async

> update_work_order_type_async(tenant_id, id, api_version, x_api_version, work_order_type_update_dto)
Update a work order type

Updates an existing work order type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**work_order_type_update_dto** | Option<[**WorkOrderTypeUpdateDto**](WorkOrderTypeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

