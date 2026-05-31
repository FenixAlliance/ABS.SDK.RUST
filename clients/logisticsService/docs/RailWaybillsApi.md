# \RailWaybillsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_rail_waybill_line_async**](RailWaybillsApi.md#add_rail_waybill_line_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines | Add a line to rail waybill
[**cancel_rail_waybill_async**](RailWaybillsApi.md#cancel_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Cancel | Cancel a rail waybill
[**create_rail_waybill_async**](RailWaybillsApi.md#create_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills | Create a rail waybill
[**delete_rail_waybill_async**](RailWaybillsApi.md#delete_rail_waybill_async) | **DELETE** /api/v2/LogisticsService/RailWaybills/{waybillId} | Delete a rail waybill
[**get_rail_waybill_by_id_async**](RailWaybillsApi.md#get_rail_waybill_by_id_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId} | Get rail waybill by ID
[**get_rail_waybill_lines_async**](RailWaybillsApi.md#get_rail_waybill_lines_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines | Get rail waybill lines
[**get_rail_waybill_lines_count_async**](RailWaybillsApi.md#get_rail_waybill_lines_count_async) | **GET** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/Count | Get rail waybill lines count
[**get_rail_waybills_async**](RailWaybillsApi.md#get_rail_waybills_async) | **GET** /api/v2/LogisticsService/RailWaybills | Get all rail waybills
[**get_rail_waybills_count_async**](RailWaybillsApi.md#get_rail_waybills_count_async) | **GET** /api/v2/LogisticsService/RailWaybills/Count | Get rail waybills count
[**issue_rail_waybill_async**](RailWaybillsApi.md#issue_rail_waybill_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/Issue | Issue a rail waybill
[**mark_rail_waybill_delivered_async**](RailWaybillsApi.md#mark_rail_waybill_delivered_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/MarkDelivered | Mark rail waybill delivered
[**mark_rail_waybill_in_transit_async**](RailWaybillsApi.md#mark_rail_waybill_in_transit_async) | **POST** /api/v2/LogisticsService/RailWaybills/{waybillId}/MarkInTransit | Mark rail waybill in transit
[**remove_rail_waybill_line_async**](RailWaybillsApi.md#remove_rail_waybill_line_async) | **DELETE** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/{lineId} | Remove a rail waybill line
[**update_rail_waybill_async**](RailWaybillsApi.md#update_rail_waybill_async) | **PUT** /api/v2/LogisticsService/RailWaybills/{waybillId} | Update a rail waybill
[**update_rail_waybill_line_async**](RailWaybillsApi.md#update_rail_waybill_line_async) | **PUT** /api/v2/LogisticsService/RailWaybills/{waybillId}/Lines/{lineId} | Update a rail waybill line



## add_rail_waybill_line_async

> models::EmptyEnvelope add_rail_waybill_line_async(tenant_id, waybill_id, api_version, x_api_version, waybill_line_create_dto)
Add a line to rail waybill

Adds a new line to a rail waybill.

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


## cancel_rail_waybill_async

> models::EmptyEnvelope cancel_rail_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Cancel a rail waybill

Cancels a rail waybill.

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


## create_rail_waybill_async

> models::EmptyEnvelope create_rail_waybill_async(tenant_id, api_version, x_api_version, rail_waybill_create_dto)
Create a rail waybill

Creates a new rail waybill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**rail_waybill_create_dto** | Option<[**RailWaybillCreateDto**](RailWaybillCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_rail_waybill_async

> models::EmptyEnvelope delete_rail_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Delete a rail waybill

Deletes a rail waybill.

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


## get_rail_waybill_by_id_async

> models::RailWaybillDtoEnvelope get_rail_waybill_by_id_async(tenant_id, waybill_id, api_version, x_api_version)
Get rail waybill by ID

Retrieves a specific rail waybill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RailWaybillDtoEnvelope**](RailWaybillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_rail_waybill_lines_async

> models::WaybillLineDtoListEnvelope get_rail_waybill_lines_async(tenant_id, waybill_id, api_version, x_api_version)
Get rail waybill lines

Retrieves all lines for a specific rail waybill.

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


## get_rail_waybill_lines_count_async

> models::Int32Envelope get_rail_waybill_lines_count_async(tenant_id, waybill_id, api_version, x_api_version)
Get rail waybill lines count

Returns the count of lines for a specific rail waybill.

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


## get_rail_waybills_async

> models::RailWaybillDtoListEnvelope get_rail_waybills_async(tenant_id, api_version, x_api_version)
Get all rail waybills

Retrieves all rail waybills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RailWaybillDtoListEnvelope**](RailWaybillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_rail_waybills_count_async

> models::Int32Envelope get_rail_waybills_count_async(tenant_id, api_version, x_api_version)
Get rail waybills count

Returns the count of rail waybills for the specified tenant.

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


## issue_rail_waybill_async

> models::EmptyEnvelope issue_rail_waybill_async(tenant_id, waybill_id, api_version, x_api_version)
Issue a rail waybill

Issues a rail waybill.

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


## mark_rail_waybill_delivered_async

> models::EmptyEnvelope mark_rail_waybill_delivered_async(tenant_id, waybill_id, api_version, x_api_version)
Mark rail waybill delivered

Marks a rail waybill as delivered.

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


## mark_rail_waybill_in_transit_async

> models::EmptyEnvelope mark_rail_waybill_in_transit_async(tenant_id, waybill_id, api_version, x_api_version)
Mark rail waybill in transit

Marks a rail waybill as in transit.

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


## remove_rail_waybill_line_async

> models::EmptyEnvelope remove_rail_waybill_line_async(tenant_id, waybill_id, line_id, api_version, x_api_version)
Remove a rail waybill line

Removes a line from a rail waybill.

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


## update_rail_waybill_async

> models::EmptyEnvelope update_rail_waybill_async(tenant_id, waybill_id, api_version, x_api_version, rail_waybill_update_dto)
Update a rail waybill

Updates an existing rail waybill.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**waybill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**rail_waybill_update_dto** | Option<[**RailWaybillUpdateDto**](RailWaybillUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_rail_waybill_line_async

> models::EmptyEnvelope update_rail_waybill_line_async(tenant_id, waybill_id, line_id, api_version, x_api_version, waybill_line_update_dto)
Update a rail waybill line

Updates an existing line on a rail waybill.

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

