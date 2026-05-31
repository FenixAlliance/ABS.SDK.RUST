# \PortsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_port_async**](PortsApi.md#create_port_async) | **POST** /api/v2/LogisticsService/Ports | Create a port
[**delete_port_async**](PortsApi.md#delete_port_async) | **DELETE** /api/v2/LogisticsService/Ports/{portId} | Delete a port
[**get_port_by_id_async**](PortsApi.md#get_port_by_id_async) | **GET** /api/v2/LogisticsService/Ports/{portId} | Get port by ID
[**get_ports_async**](PortsApi.md#get_ports_async) | **GET** /api/v2/LogisticsService/Ports | Get all ports
[**get_ports_count_async**](PortsApi.md#get_ports_count_async) | **GET** /api/v2/LogisticsService/Ports/Count | Get ports count
[**update_port_async**](PortsApi.md#update_port_async) | **PUT** /api/v2/LogisticsService/Ports/{portId} | Update a port



## create_port_async

> models::EmptyEnvelope create_port_async(tenant_id, api_version, x_api_version, port_create_dto)
Create a port

Creates a new port for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**port_create_dto** | Option<[**PortCreateDto**](PortCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_port_async

> models::EmptyEnvelope delete_port_async(tenant_id, port_id, api_version, x_api_version)
Delete a port

Deletes a port.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**port_id** | **uuid::Uuid** |  | [required] |
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


## get_port_by_id_async

> models::PortDtoEnvelope get_port_by_id_async(tenant_id, port_id, api_version, x_api_version)
Get port by ID

Retrieves a specific port by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**port_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PortDtoEnvelope**](PortDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_ports_async

> models::PortDtoListEnvelope get_ports_async(tenant_id, api_version, x_api_version)
Get all ports

Retrieves all ports for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PortDtoListEnvelope**](PortDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_ports_count_async

> models::Int32Envelope get_ports_count_async(tenant_id, api_version, x_api_version)
Get ports count

Returns the count of ports for the specified tenant.

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


## update_port_async

> models::EmptyEnvelope update_port_async(tenant_id, port_id, api_version, x_api_version, port_update_dto)
Update a port

Updates an existing port.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**port_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**port_update_dto** | Option<[**PortUpdateDto**](PortUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

