# \SalesLiteraturesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_sales_literatures_async**](SalesLiteraturesApi.md#count_sales_literatures_async) | **GET** /api/v2/DealsService/SalesLiteratures/Count | Get sales literatures count
[**create_sales_literature_async**](SalesLiteraturesApi.md#create_sales_literature_async) | **POST** /api/v2/DealsService/SalesLiteratures | Create a sales literature
[**delete_sales_literature_async**](SalesLiteraturesApi.md#delete_sales_literature_async) | **DELETE** /api/v2/DealsService/SalesLiteratures/{salesLiteratureId} | Delete a sales literature
[**get_extended_sales_literatures_async**](SalesLiteraturesApi.md#get_extended_sales_literatures_async) | **GET** /api/v2/DealsService/SalesLiteratures/Extended | Get extended sales literatures
[**get_sales_literature_async**](SalesLiteraturesApi.md#get_sales_literature_async) | **GET** /api/v2/DealsService/SalesLiteratures/{salesLiteratureId} | Get sales literature by ID
[**get_sales_literatures_async**](SalesLiteraturesApi.md#get_sales_literatures_async) | **GET** /api/v2/DealsService/SalesLiteratures | Get sales literatures
[**update_sales_literature_async**](SalesLiteraturesApi.md#update_sales_literature_async) | **PUT** /api/v2/DealsService/SalesLiteratures/{salesLiteratureId} | Update a sales literature



## count_sales_literatures_async

> models::Int32Envelope count_sales_literatures_async(tenant_id)
Get sales literatures count

Returns the total count of sales literatures for the specified tenant with OData filter support.

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


## create_sales_literature_async

> models::EmptyEnvelope create_sales_literature_async(tenant_id, sales_literature_create_dto)
Create a sales literature

Creates a new sales literature for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**sales_literature_create_dto** | Option<[**SalesLiteratureCreateDto**](SalesLiteratureCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_sales_literature_async

> models::EmptyEnvelope delete_sales_literature_async(tenant_id, sales_literature_id)
Delete a sales literature

Deletes an existing sales literature by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**sales_literature_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_sales_literatures_async

> models::ExtendedSalesLiteratureDtoListEnvelope get_extended_sales_literatures_async(tenant_id)
Get extended sales literatures

Retrieves a list of sales literatures with extended details for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedSalesLiteratureDtoListEnvelope**](ExtendedSalesLiteratureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sales_literature_async

> models::SalesLiteratureDtoEnvelope get_sales_literature_async(tenant_id, sales_literature_id)
Get sales literature by ID

Retrieves a single sales literature by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**sales_literature_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::SalesLiteratureDtoEnvelope**](SalesLiteratureDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sales_literatures_async

> models::SalesLiteratureDtoListEnvelope get_sales_literatures_async(tenant_id)
Get sales literatures

Retrieves a list of sales literatures for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::SalesLiteratureDtoListEnvelope**](SalesLiteratureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_sales_literature_async

> models::EmptyEnvelope update_sales_literature_async(tenant_id, sales_literature_id, sales_literature_update_dto)
Update a sales literature

Updates an existing sales literature by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**sales_literature_id** | **uuid::Uuid** |  | [required] |
**sales_literature_update_dto** | Option<[**SalesLiteratureUpdateDto**](SalesLiteratureUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

