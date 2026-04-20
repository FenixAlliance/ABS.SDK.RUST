# \DealUnitsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_deal_unit_async**](DealUnitsApi.md#calculate_deal_unit_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Calculate | Calculate a deal unit
[**calculate_deal_unit_line_async**](DealUnitsApi.md#calculate_deal_unit_line_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId}/Calculate | Calculate a deal unit line
[**create_deal_unit_async**](DealUnitsApi.md#create_deal_unit_async) | **POST** /api/v2/DealsService/DealUnits | Create a deal unit
[**create_get_deal_unit_lines_async**](DealUnitsApi.md#create_get_deal_unit_lines_async) | **POST** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines | Create a deal unit line
[**delete_deal_unit_async**](DealUnitsApi.md#delete_deal_unit_async) | **DELETE** /api/v2/DealsService/DealUnits/{dealUnitId} | Delete a deal unit
[**delete_deal_unit_price_async**](DealUnitsApi.md#delete_deal_unit_price_async) | **DELETE** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Delete a deal unit line
[**get_deal_unit_async**](DealUnitsApi.md#get_deal_unit_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId} | Get deal unit by ID
[**get_deal_unit_lines_async**](DealUnitsApi.md#get_deal_unit_lines_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines | Get deal unit lines
[**get_deal_unit_lines_count_async**](DealUnitsApi.md#get_deal_unit_lines_count_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/Count | Get deal unit lines count
[**get_deal_unit_price_async**](DealUnitsApi.md#get_deal_unit_price_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Get a deal unit line by ID
[**get_deal_units_async**](DealUnitsApi.md#get_deal_units_async) | **GET** /api/v2/DealsService/DealUnits | Get deal units
[**get_deal_units_count_async**](DealUnitsApi.md#get_deal_units_count_async) | **GET** /api/v2/DealsService/DealUnits/Count | Get deal units count
[**get_extended_deal_unit_async**](DealUnitsApi.md#get_extended_deal_unit_async) | **GET** /api/v2/DealsService/DealUnits/{dealUnitId}/Extended | Get extended deal unit by ID
[**get_extended_deal_units_async**](DealUnitsApi.md#get_extended_deal_units_async) | **GET** /api/v2/DealsService/DealUnits/Extended | Get extended deal units
[**update_deal_unit_async**](DealUnitsApi.md#update_deal_unit_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId} | Update a deal unit
[**update_deal_unit_price_async**](DealUnitsApi.md#update_deal_unit_price_async) | **PUT** /api/v2/DealsService/DealUnits/{dealUnitId}/Lines/{dealUnitLineId} | Update a deal unit line



## calculate_deal_unit_async

> models::EmptyEnvelope calculate_deal_unit_async(tenant_id, deal_unit_id)
Calculate a deal unit

Triggers recalculation of totals and derived values for a specific deal unit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## calculate_deal_unit_line_async

> models::EmptyEnvelope calculate_deal_unit_line_async(tenant_id, deal_unit_id, deal_unit_line_id)
Calculate a deal unit line

Triggers recalculation of totals and derived values for a specific deal unit line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_deal_unit_async

> models::EmptyEnvelope create_deal_unit_async(tenant_id, deal_unit_create_dto)
Create a deal unit

Creates a new deal unit for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_create_dto** | Option<[**DealUnitCreateDto**](DealUnitCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_get_deal_unit_lines_async

> models::EmptyEnvelope create_get_deal_unit_lines_async(tenant_id, deal_unit_id, deal_unit_line_create_dto)
Create a deal unit line

Creates a new line within a specific deal unit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_create_dto** | Option<[**DealUnitLineCreateDto**](DealUnitLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_deal_unit_async

> models::EmptyEnvelope delete_deal_unit_async(tenant_id, deal_unit_id)
Delete a deal unit

Deletes an existing deal unit by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_deal_unit_price_async

> models::EmptyEnvelope delete_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)
Delete a deal unit line

Deletes an existing line from a specific deal unit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_unit_async

> models::DealUnitDtoEnvelope get_deal_unit_async(tenant_id, deal_unit_id)
Get deal unit by ID

Retrieves a single deal unit by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DealUnitDtoEnvelope**](DealUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_unit_lines_async

> models::DealUnitLineDtoListEnvelope get_deal_unit_lines_async(tenant_id, deal_unit_id, item_id)
Get deal unit lines

Retrieves a list of lines for a specific deal unit with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::DealUnitLineDtoListEnvelope**](DealUnitLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_unit_lines_count_async

> models::Int32Envelope get_deal_unit_lines_count_async(tenant_id, deal_unit_id)
Get deal unit lines count

Returns the total count of lines for a specific deal unit with OData filter support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_unit_price_async

> models::DealUnitLineDtoEnvelope get_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id)
Get a deal unit line by ID

Retrieves a single deal unit line by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DealUnitLineDtoEnvelope**](DealUnitLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_units_async

> models::DealUnitDtoListEnvelope get_deal_units_async(tenant_id)
Get deal units

Retrieves a list of deal units for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DealUnitDtoListEnvelope**](DealUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_deal_units_count_async

> models::Int32Envelope get_deal_units_count_async(tenant_id)
Get deal units count

Returns the total count of deal units for the specified tenant with OData filter support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_deal_unit_async

> models::ExtendedDealUnitDtoEnvelope get_extended_deal_unit_async(tenant_id, deal_unit_id)
Get extended deal unit by ID

Retrieves a single deal unit with extended details by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedDealUnitDtoEnvelope**](ExtendedDealUnitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_deal_units_async

> models::ExtendedDealUnitDtoListEnvelope get_extended_deal_units_async(tenant_id)
Get extended deal units

Retrieves a list of deal units with extended details for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedDealUnitDtoListEnvelope**](ExtendedDealUnitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_deal_unit_async

> models::EmptyEnvelope update_deal_unit_async(tenant_id, deal_unit_id, deal_unit_update_dto)
Update a deal unit

Updates an existing deal unit by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_update_dto** | Option<[**DealUnitUpdateDto**](DealUnitUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_deal_unit_price_async

> models::EmptyEnvelope update_deal_unit_price_async(tenant_id, deal_unit_id, deal_unit_line_id, deal_unit_line_update_dto)
Update a deal unit line

Updates an existing line within a specific deal unit.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**deal_unit_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_id** | **uuid::Uuid** |  | [required] |
**deal_unit_line_update_dto** | Option<[**DealUnitLineUpdateDto**](DealUnitLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

