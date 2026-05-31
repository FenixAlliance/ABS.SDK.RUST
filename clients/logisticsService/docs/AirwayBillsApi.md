# \AirwayBillsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_airway_bill_line_async**](AirwayBillsApi.md#add_airway_bill_line_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Lines | Add a line to airway bill
[**cancel_airway_bill_async**](AirwayBillsApi.md#cancel_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Cancel | Cancel an airway bill
[**create_airway_bill_async**](AirwayBillsApi.md#create_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills | Create an airway bill
[**delete_airway_bill_async**](AirwayBillsApi.md#delete_airway_bill_async) | **DELETE** /api/v2/LogisticsService/AirwayBills/{billId} | Delete an airway bill
[**get_airway_bill_by_id_async**](AirwayBillsApi.md#get_airway_bill_by_id_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId} | Get airway bill by ID
[**get_airway_bill_lines_async**](AirwayBillsApi.md#get_airway_bill_lines_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId}/Lines | Get airway bill lines
[**get_airway_bill_lines_count_async**](AirwayBillsApi.md#get_airway_bill_lines_count_async) | **GET** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/Count | Get airway bill lines count
[**get_airway_bills_async**](AirwayBillsApi.md#get_airway_bills_async) | **GET** /api/v2/LogisticsService/AirwayBills | Get all airway bills
[**get_airway_bills_count_async**](AirwayBillsApi.md#get_airway_bills_count_async) | **GET** /api/v2/LogisticsService/AirwayBills/Count | Get airway bills count
[**issue_airway_bill_async**](AirwayBillsApi.md#issue_airway_bill_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/Issue | Issue an airway bill
[**mark_airway_bill_arrived_async**](AirwayBillsApi.md#mark_airway_bill_arrived_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkArrived | Mark airway bill arrived
[**mark_airway_bill_delivered_async**](AirwayBillsApi.md#mark_airway_bill_delivered_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkDelivered | Mark airway bill delivered
[**mark_airway_bill_in_transit_async**](AirwayBillsApi.md#mark_airway_bill_in_transit_async) | **POST** /api/v2/LogisticsService/AirwayBills/{billId}/MarkInTransit | Mark airway bill in transit
[**remove_airway_bill_line_async**](AirwayBillsApi.md#remove_airway_bill_line_async) | **DELETE** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/{lineId} | Remove an airway bill line
[**update_airway_bill_async**](AirwayBillsApi.md#update_airway_bill_async) | **PUT** /api/v2/LogisticsService/AirwayBills/{billId} | Update an airway bill
[**update_airway_bill_line_async**](AirwayBillsApi.md#update_airway_bill_line_async) | **PUT** /api/v2/LogisticsService/AirwayBills/{billId}/Lines/{lineId} | Update an airway bill line



## add_airway_bill_line_async

> models::EmptyEnvelope add_airway_bill_line_async(tenant_id, bill_id, api_version, x_api_version, waybill_line_create_dto)
Add a line to airway bill

Adds a new line to an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**waybill_line_create_dto** | Option<[**WaybillLineCreateDto**](WaybillLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cancel_airway_bill_async

> models::EmptyEnvelope cancel_airway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Cancel an airway bill

Cancels an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## create_airway_bill_async

> models::EmptyEnvelope create_airway_bill_async(tenant_id, api_version, x_api_version, airway_bill_create_dto)
Create an airway bill

Creates a new airway bill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**airway_bill_create_dto** | Option<[**AirwayBillCreateDto**](AirwayBillCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_airway_bill_async

> models::EmptyEnvelope delete_airway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Delete an airway bill

Deletes an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## get_airway_bill_by_id_async

> models::AirwayBillDtoEnvelope get_airway_bill_by_id_async(tenant_id, bill_id, api_version, x_api_version)
Get airway bill by ID

Retrieves a specific airway bill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AirwayBillDtoEnvelope**](AirwayBillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_airway_bill_lines_async

> models::WaybillLineDtoListEnvelope get_airway_bill_lines_async(tenant_id, bill_id, api_version, x_api_version)
Get airway bill lines

Retrieves all lines for a specific airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WaybillLineDtoListEnvelope**](WaybillLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_airway_bill_lines_count_async

> models::Int32Envelope get_airway_bill_lines_count_async(tenant_id, bill_id, api_version, x_api_version)
Get airway bill lines count

Returns the count of lines for a specific airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## get_airway_bills_async

> models::AirwayBillDtoListEnvelope get_airway_bills_async(tenant_id, api_version, x_api_version)
Get all airway bills

Retrieves all airway bills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AirwayBillDtoListEnvelope**](AirwayBillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_airway_bills_count_async

> models::Int32Envelope get_airway_bills_count_async(tenant_id, api_version, x_api_version)
Get airway bills count

Returns the count of airway bills for the specified tenant.

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


## issue_airway_bill_async

> models::EmptyEnvelope issue_airway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Issue an airway bill

Issues an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## mark_airway_bill_arrived_async

> models::EmptyEnvelope mark_airway_bill_arrived_async(tenant_id, bill_id, api_version, x_api_version)
Mark airway bill arrived

Marks an airway bill as arrived.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## mark_airway_bill_delivered_async

> models::EmptyEnvelope mark_airway_bill_delivered_async(tenant_id, bill_id, api_version, x_api_version)
Mark airway bill delivered

Marks an airway bill as delivered.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## mark_airway_bill_in_transit_async

> models::EmptyEnvelope mark_airway_bill_in_transit_async(tenant_id, bill_id, api_version, x_api_version)
Mark airway bill in transit

Marks an airway bill as in transit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
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


## remove_airway_bill_line_async

> models::EmptyEnvelope remove_airway_bill_line_async(tenant_id, bill_id, line_id, api_version, x_api_version)
Remove an airway bill line

Removes a line from an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
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


## update_airway_bill_async

> models::EmptyEnvelope update_airway_bill_async(tenant_id, bill_id, api_version, x_api_version, airway_bill_update_dto)
Update an airway bill

Updates an existing airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**airway_bill_update_dto** | Option<[**AirwayBillUpdateDto**](AirwayBillUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_airway_bill_line_async

> models::EmptyEnvelope update_airway_bill_line_async(tenant_id, bill_id, line_id, api_version, x_api_version, waybill_line_update_dto)
Update an airway bill line

Updates an existing line on an airway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**waybill_line_update_dto** | Option<[**WaybillLineUpdateDto**](WaybillLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

