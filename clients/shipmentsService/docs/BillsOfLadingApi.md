# \BillsOfLadingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_bill_of_lading_async**](BillsOfLadingApi.md#create_bill_of_lading_async) | **POST** /api/v2/ShipmentsService/BillsOfLading | Create a bill of lading
[**create_bill_of_lading_line_async**](BillsOfLadingApi.md#create_bill_of_lading_line_async) | **POST** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines | Create a bill of lading line
[**delete_bill_of_lading_async**](BillsOfLadingApi.md#delete_bill_of_lading_async) | **DELETE** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Delete a bill of lading
[**delete_bill_of_lading_line_async**](BillsOfLadingApi.md#delete_bill_of_lading_line_async) | **DELETE** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Delete a bill of lading line
[**get_bill_of_lading_by_id_async**](BillsOfLadingApi.md#get_bill_of_lading_by_id_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Get bill of lading by ID
[**get_bill_of_lading_line_by_id_async**](BillsOfLadingApi.md#get_bill_of_lading_line_by_id_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Get bill of lading line by ID
[**get_bill_of_lading_lines_async**](BillsOfLadingApi.md#get_bill_of_lading_lines_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines | Get bill of lading lines
[**get_bill_of_lading_lines_count_async**](BillsOfLadingApi.md#get_bill_of_lading_lines_count_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/Count | Get bill of lading lines count
[**get_bills_of_lading_async**](BillsOfLadingApi.md#get_bills_of_lading_async) | **GET** /api/v2/ShipmentsService/BillsOfLading | Get all bills of lading
[**get_bills_of_lading_count_async**](BillsOfLadingApi.md#get_bills_of_lading_count_async) | **GET** /api/v2/ShipmentsService/BillsOfLading/Count | Get bills of lading count
[**update_bill_of_lading_async**](BillsOfLadingApi.md#update_bill_of_lading_async) | **PUT** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId} | Update a bill of lading
[**update_bill_of_lading_line_async**](BillsOfLadingApi.md#update_bill_of_lading_line_async) | **PUT** /api/v2/ShipmentsService/BillsOfLading/{billOfLadingId}/Lines/{lineId} | Update a bill of lading line



## create_bill_of_lading_async

> models::EmptyEnvelope create_bill_of_lading_async(tenant_id, api_version, x_api_version, bill_of_lading_create_dto)
Create a bill of lading

Creates a new bill of lading for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bill_of_lading_create_dto** | Option<[**BillOfLadingCreateDto**](BillOfLadingCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_bill_of_lading_line_async

> models::EmptyEnvelope create_bill_of_lading_line_async(tenant_id, bill_of_lading_id, api_version, x_api_version, bill_of_lading_line_create_dto)
Create a bill of lading line

Creates a new line for a bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bill_of_lading_line_create_dto** | Option<[**BillOfLadingLineCreateDto**](BillOfLadingLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_bill_of_lading_async

> models::EmptyEnvelope delete_bill_of_lading_async(tenant_id, bill_of_lading_id, api_version, x_api_version)
Delete a bill of lading

Deletes a bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
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


## delete_bill_of_lading_line_async

> models::EmptyEnvelope delete_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, api_version, x_api_version)
Delete a bill of lading line

Deletes a line from a bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
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


## get_bill_of_lading_by_id_async

> models::BillOfLadingDtoEnvelope get_bill_of_lading_by_id_async(tenant_id, bill_of_lading_id, api_version, x_api_version)
Get bill of lading by ID

Retrieves a specific bill of lading by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillOfLadingDtoEnvelope**](BillOfLadingDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_bill_of_lading_line_by_id_async

> models::BillOfLadingLineDtoEnvelope get_bill_of_lading_line_by_id_async(tenant_id, bill_of_lading_id, line_id, api_version, x_api_version)
Get bill of lading line by ID

Retrieves a specific line from a bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillOfLadingLineDtoEnvelope**](BillOfLadingLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_bill_of_lading_lines_async

> models::BillOfLadingLineDtoListEnvelope get_bill_of_lading_lines_async(tenant_id, bill_of_lading_id, api_version, x_api_version)
Get bill of lading lines

Retrieves all lines for a specific bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillOfLadingLineDtoListEnvelope**](BillOfLadingLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_bill_of_lading_lines_count_async

> models::Int32Envelope get_bill_of_lading_lines_count_async(tenant_id, bill_of_lading_id, api_version, x_api_version)
Get bill of lading lines count

Returns the count of lines for a specific bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
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


## get_bills_of_lading_async

> models::BillOfLadingDtoListEnvelope get_bills_of_lading_async(tenant_id, api_version, x_api_version)
Get all bills of lading

Retrieves all bills of lading for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillOfLadingDtoListEnvelope**](BillOfLadingDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_bills_of_lading_count_async

> models::Int32Envelope get_bills_of_lading_count_async(tenant_id, api_version, x_api_version)
Get bills of lading count

Returns the count of bills of lading for the specified tenant.

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


## update_bill_of_lading_async

> models::EmptyEnvelope update_bill_of_lading_async(tenant_id, bill_of_lading_id, api_version, x_api_version, bill_of_lading_update_dto)
Update a bill of lading

Updates an existing bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bill_of_lading_update_dto** | Option<[**BillOfLadingUpdateDto**](BillOfLadingUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_bill_of_lading_line_async

> models::EmptyEnvelope update_bill_of_lading_line_async(tenant_id, bill_of_lading_id, line_id, api_version, x_api_version, bill_of_lading_line_update_dto)
Update a bill of lading line

Updates an existing line on a bill of lading.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**bill_of_lading_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bill_of_lading_line_update_dto** | Option<[**BillOfLadingLineUpdateDto**](BillOfLadingLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

