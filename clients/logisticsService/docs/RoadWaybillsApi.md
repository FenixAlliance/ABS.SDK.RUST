# \RoadWaybillsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_road_waybill_line_async**](RoadWaybillsApi.md#add_road_waybill_line_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines | Add a line to road waybill
[**cancel_road_waybill_async**](RoadWaybillsApi.md#cancel_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Cancel | Cancel a road waybill
[**create_road_waybill_async**](RoadWaybillsApi.md#create_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills | Create a road waybill
[**delete_road_waybill_async**](RoadWaybillsApi.md#delete_road_waybill_async) | **DELETE** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Delete a road waybill
[**dispute_road_waybill_async**](RoadWaybillsApi.md#dispute_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Dispute | Dispute a road waybill
[**get_road_waybill_by_id_async**](RoadWaybillsApi.md#get_road_waybill_by_id_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Get road waybill by ID
[**get_road_waybill_lines_async**](RoadWaybillsApi.md#get_road_waybill_lines_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines | Get road waybill lines
[**get_road_waybill_lines_count_async**](RoadWaybillsApi.md#get_road_waybill_lines_count_async) | **GET** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/Count | Get road waybill lines count
[**get_road_waybills_async**](RoadWaybillsApi.md#get_road_waybills_async) | **GET** /api/v2/LogisticsService/RoadWaybills | Get all road waybills
[**get_road_waybills_count_async**](RoadWaybillsApi.md#get_road_waybills_count_async) | **GET** /api/v2/LogisticsService/RoadWaybills/Count | Get road waybills count
[**issue_road_waybill_async**](RoadWaybillsApi.md#issue_road_waybill_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Issue | Issue a road waybill
[**mark_road_waybill_delivered_async**](RoadWaybillsApi.md#mark_road_waybill_delivered_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/MarkDelivered | Mark road waybill delivered
[**mark_road_waybill_in_transit_async**](RoadWaybillsApi.md#mark_road_waybill_in_transit_async) | **POST** /api/v2/LogisticsService/RoadWaybills/{waybillId}/MarkInTransit | Mark road waybill in transit
[**remove_road_waybill_line_async**](RoadWaybillsApi.md#remove_road_waybill_line_async) | **DELETE** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/{lineId} | Remove a road waybill line
[**update_road_waybill_async**](RoadWaybillsApi.md#update_road_waybill_async) | **PUT** /api/v2/LogisticsService/RoadWaybills/{waybillId} | Update a road waybill
[**update_road_waybill_line_async**](RoadWaybillsApi.md#update_road_waybill_line_async) | **PUT** /api/v2/LogisticsService/RoadWaybills/{waybillId}/Lines/{lineId} | Update a road waybill line



## add_road_waybill_line_async

> models::EmptyEnvelope add_road_waybill_line_async(tenant_id, waybill_id, api_version, x_api_version, waybill_line_create_dto)
Add a line to road waybill

Adds a new line to a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## cancel_road_waybill_async

> models::EmptyEnvelope cancel_road_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Cancel a road waybill

Cancels a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## create_road_waybill_async

> models::EmptyEnvelope create_road_waybill_async(tenant_id, api_version, x_api_version, road_waybill_create_dto)
Create a road waybill

Creates a new road waybill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**road_waybill_create_dto** | Option<[**RoadWaybillCreateDto**](RoadWaybillCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_road_waybill_async

> models::EmptyEnvelope delete_road_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Delete a road waybill

Deletes a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## dispute_road_waybill_async

> models::EmptyEnvelope dispute_road_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Dispute a road waybill

Disputes a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## get_road_waybill_by_id_async

> models::RoadWaybillDtoEnvelope get_road_waybill_by_id_async(tenant_id, waybill_id, api_version, x_api_version)
Get road waybill by ID

Retrieves a specific road waybill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RoadWaybillDtoEnvelope**](RoadWaybillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_road_waybill_lines_async

> models::WaybillLineDtoListEnvelope get_road_waybill_lines_async(tenant_id, waybill_id, api_version, x_api_version)
Get road waybill lines

Retrieves all lines for a specific road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## get_road_waybill_lines_count_async

> models::Int32Envelope get_road_waybill_lines_count_async(tenant_id, waybill_id, api_version, x_api_version)
Get road waybill lines count

Returns the count of lines for a specific road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## get_road_waybills_async

> models::RoadWaybillDtoListEnvelope get_road_waybills_async(tenant_id, api_version, x_api_version)
Get all road waybills

Retrieves all road waybills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RoadWaybillDtoListEnvelope**](RoadWaybillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_road_waybills_count_async

> models::Int32Envelope get_road_waybills_count_async(tenant_id, api_version, x_api_version)
Get road waybills count

Returns the count of road waybills for the specified tenant.

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


## issue_road_waybill_async

> models::EmptyEnvelope issue_road_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Issue a road waybill

Issues a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## mark_road_waybill_delivered_async

> models::EmptyEnvelope mark_road_waybill_delivered_async(tenant_id, waybill_id, api_version, x_api_version)
Mark road waybill delivered

Marks a road waybill as delivered.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## mark_road_waybill_in_transit_async

> models::EmptyEnvelope mark_road_waybill_in_transit_async(tenant_id, waybill_id, api_version, x_api_version)
Mark road waybill in transit

Marks a road waybill as in transit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## remove_road_waybill_line_async

> models::EmptyEnvelope remove_road_waybill_line_async(tenant_id, waybill_id, line_id, api_version, x_api_version)
Remove a road waybill line

Removes a line from a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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


## update_road_waybill_async

> models::EmptyEnvelope update_road_waybill_async(tenant_id, waybill_id, api_version, x_api_version, road_waybill_update_dto)
Update a road waybill

Updates an existing road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**road_waybill_update_dto** | Option<[**RoadWaybillUpdateDto**](RoadWaybillUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_road_waybill_line_async

> models::EmptyEnvelope update_road_waybill_line_async(tenant_id, waybill_id, line_id, api_version, x_api_version, waybill_line_update_dto)
Update a road waybill line

Updates an existing line on a road waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
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

