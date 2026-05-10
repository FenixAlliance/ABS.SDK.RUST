# \ShipmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipment_async**](ShipmentsApi.md#create_shipment_async) | **POST** /api/v2/ShipmentsService/Shipments | Create a shipment
[**delete_shipment_async**](ShipmentsApi.md#delete_shipment_async) | **DELETE** /api/v2/ShipmentsService/Shipments/{shipmentId} | Delete a shipment
[**get_shipment_by_id_async**](ShipmentsApi.md#get_shipment_by_id_async) | **GET** /api/v2/ShipmentsService/Shipments/{shipmentId} | Get shipment by ID
[**get_shipments_async**](ShipmentsApi.md#get_shipments_async) | **GET** /api/v2/ShipmentsService/Shipments | Get all shipments
[**get_shipments_count_async**](ShipmentsApi.md#get_shipments_count_async) | **GET** /api/v2/ShipmentsService/Shipments/Count | Get shipments count
[**update_shipment_async**](ShipmentsApi.md#update_shipment_async) | **PUT** /api/v2/ShipmentsService/Shipments/{shipmentId} | Update a shipment



## create_shipment_async

> create_shipment_async(tenant_id, api_version, x_api_version, shipment_create_dto)
Create a shipment

Creates a new shipment for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipment_create_dto** | Option<[**ShipmentCreateDto**](ShipmentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipment_async

> delete_shipment_async(tenant_id, shipment_id, api_version, x_api_version)
Delete a shipment

Deletes a shipment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shipment_id** | **uuid::Uuid** |  | [required] |
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


## get_shipment_by_id_async

> models::ShipmentDtoEnvelope get_shipment_by_id_async(tenant_id, shipment_id, api_version, x_api_version)
Get shipment by ID

Retrieves a specific shipment by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shipment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShipmentDtoEnvelope**](ShipmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipments_async

> models::ShipmentDtoListEnvelope get_shipments_async(tenant_id, api_version, x_api_version)
Get all shipments

Retrieves all shipments for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShipmentDtoListEnvelope**](ShipmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipments_count_async

> models::Int32Envelope get_shipments_count_async(tenant_id, api_version, x_api_version)
Get shipments count

Returns the count of shipments for the specified tenant.

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


## update_shipment_async

> update_shipment_async(tenant_id, shipment_id, api_version, x_api_version, shipment_update_dto)
Update a shipment

Updates an existing shipment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shipment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipment_update_dto** | Option<[**ShipmentUpdateDto**](ShipmentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

