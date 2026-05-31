# \SeawayBillsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_seaway_bill_line_async**](SeawayBillsApi.md#add_seaway_bill_line_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Lines | Add a line to seaway bill
[**cancel_seaway_bill_async**](SeawayBillsApi.md#cancel_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Cancel | Cancel a seaway bill
[**create_seaway_bill_async**](SeawayBillsApi.md#create_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills | Create a seaway bill
[**delete_seaway_bill_async**](SeawayBillsApi.md#delete_seaway_bill_async) | **DELETE** /api/v2/LogisticsService/SeawayBills/{billId} | Delete a seaway bill
[**get_seaway_bill_by_id_async**](SeawayBillsApi.md#get_seaway_bill_by_id_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId} | Get seaway bill by ID
[**get_seaway_bill_lines_async**](SeawayBillsApi.md#get_seaway_bill_lines_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId}/Lines | Get seaway bill lines
[**get_seaway_bill_lines_count_async**](SeawayBillsApi.md#get_seaway_bill_lines_count_async) | **GET** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/Count | Get seaway bill lines count
[**get_seaway_bills_async**](SeawayBillsApi.md#get_seaway_bills_async) | **GET** /api/v2/LogisticsService/SeawayBills | Get all seaway bills
[**get_seaway_bills_count_async**](SeawayBillsApi.md#get_seaway_bills_count_async) | **GET** /api/v2/LogisticsService/SeawayBills/Count | Get seaway bills count
[**issue_seaway_bill_async**](SeawayBillsApi.md#issue_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Issue | Issue a seaway bill
[**mark_seaway_bill_arrived_async**](SeawayBillsApi.md#mark_seaway_bill_arrived_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/MarkArrived | Mark seaway bill arrived
[**mark_seaway_bill_in_transit_async**](SeawayBillsApi.md#mark_seaway_bill_in_transit_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/MarkInTransit | Mark seaway bill in transit
[**release_seaway_bill_async**](SeawayBillsApi.md#release_seaway_bill_async) | **POST** /api/v2/LogisticsService/SeawayBills/{billId}/Release | Release a seaway bill
[**remove_seaway_bill_line_async**](SeawayBillsApi.md#remove_seaway_bill_line_async) | **DELETE** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/{lineId} | Remove a seaway bill line
[**update_seaway_bill_async**](SeawayBillsApi.md#update_seaway_bill_async) | **PUT** /api/v2/LogisticsService/SeawayBills/{billId} | Update a seaway bill
[**update_seaway_bill_line_async**](SeawayBillsApi.md#update_seaway_bill_line_async) | **PUT** /api/v2/LogisticsService/SeawayBills/{billId}/Lines/{lineId} | Update a seaway bill line



## add_seaway_bill_line_async

> models::EmptyEnvelope add_seaway_bill_line_async(tenant_id, bill_id, api_version, x_api_version, waybill_line_create_dto)
Add a line to seaway bill

Adds a new line to a seaway bill.

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


## cancel_seaway_bill_async

> models::EmptyEnvelope cancel_seaway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Cancel a seaway bill

Cancels a seaway bill.

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


## create_seaway_bill_async

> models::EmptyEnvelope create_seaway_bill_async(tenant_id, api_version, x_api_version, seaway_bill_create_dto)
Create a seaway bill

Creates a new seaway bill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**seaway_bill_create_dto** | Option<[**SeawayBillCreateDto**](SeawayBillCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_seaway_bill_async

> models::EmptyEnvelope delete_seaway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Delete a seaway bill

Deletes a seaway bill.

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


## get_seaway_bill_by_id_async

> models::SeawayBillDtoEnvelope get_seaway_bill_by_id_async(tenant_id, bill_id, api_version, x_api_version)
Get seaway bill by ID

Retrieves a specific seaway bill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SeawayBillDtoEnvelope**](SeawayBillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_seaway_bill_lines_async

> models::WaybillLineDtoListEnvelope get_seaway_bill_lines_async(tenant_id, bill_id, api_version, x_api_version)
Get seaway bill lines

Retrieves all lines for a specific seaway bill.

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


## get_seaway_bill_lines_count_async

> models::Int32Envelope get_seaway_bill_lines_count_async(tenant_id, bill_id, api_version, x_api_version)
Get seaway bill lines count

Returns the count of lines for a specific seaway bill.

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


## get_seaway_bills_async

> models::SeawayBillDtoListEnvelope get_seaway_bills_async(tenant_id, api_version, x_api_version)
Get all seaway bills

Retrieves all seaway bills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SeawayBillDtoListEnvelope**](SeawayBillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_seaway_bills_count_async

> models::Int32Envelope get_seaway_bills_count_async(tenant_id, api_version, x_api_version)
Get seaway bills count

Returns the count of seaway bills for the specified tenant.

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


## issue_seaway_bill_async

> models::EmptyEnvelope issue_seaway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Issue a seaway bill

Issues a seaway bill.

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


## mark_seaway_bill_arrived_async

> models::EmptyEnvelope mark_seaway_bill_arrived_async(tenant_id, bill_id, api_version, x_api_version)
Mark seaway bill arrived

Marks a seaway bill as arrived.

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


## mark_seaway_bill_in_transit_async

> models::EmptyEnvelope mark_seaway_bill_in_transit_async(tenant_id, bill_id, api_version, x_api_version)
Mark seaway bill in transit

Marks a seaway bill as in transit.

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


## release_seaway_bill_async

> models::EmptyEnvelope release_seaway_bill_async(tenant_id, bill_id, api_version, x_api_version)
Release a seaway bill

Releases a seaway bill.

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


## remove_seaway_bill_line_async

> models::EmptyEnvelope remove_seaway_bill_line_async(tenant_id, bill_id, line_id, api_version, x_api_version)
Remove a seaway bill line

Removes a line from a seaway bill.

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


## update_seaway_bill_async

> models::EmptyEnvelope update_seaway_bill_async(tenant_id, bill_id, api_version, x_api_version, seaway_bill_update_dto)
Update a seaway bill

Updates an existing seaway bill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**seaway_bill_update_dto** | Option<[**SeawayBillUpdateDto**](SeawayBillUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_seaway_bill_line_async

> models::EmptyEnvelope update_seaway_bill_line_async(tenant_id, bill_id, line_id, api_version, x_api_version, waybill_line_update_dto)
Update a seaway bill line

Updates an existing line on a seaway bill.

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

