# \PointOfSalesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_point_of_sales_async**](PointOfSalesApi.md#count_point_of_sales_async) | **GET** /api/v2/SalesService/PointOfSales/Count | Get point of sales count
[**create_point_of_sale_async**](PointOfSalesApi.md#create_point_of_sale_async) | **POST** /api/v2/SalesService/PointOfSales | Create a point of sale
[**delete_point_of_sale_async**](PointOfSalesApi.md#delete_point_of_sale_async) | **DELETE** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Delete a point of sale
[**get_point_of_sale_async**](PointOfSalesApi.md#get_point_of_sale_async) | **GET** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Get point of sale by ID
[**get_point_of_sales_async**](PointOfSalesApi.md#get_point_of_sales_async) | **GET** /api/v2/SalesService/PointOfSales | Get point of sales
[**update_point_of_sale_async**](PointOfSalesApi.md#update_point_of_sale_async) | **PUT** /api/v2/SalesService/PointOfSales/{pointOfSaleId} | Update a point of sale



## count_point_of_sales_async

> models::Int32Envelope count_point_of_sales_async(tenant_id)
Get point of sales count

Returns the total count of point of sales for the specified tenant with OData filter support.

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


## create_point_of_sale_async

> models::EmptyEnvelope create_point_of_sale_async(tenant_id, point_of_sale_create_dto)
Create a point of sale

Creates a new point of sale for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**point_of_sale_create_dto** | Option<[**PointOfSaleCreateDto**](PointOfSaleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_point_of_sale_async

> models::EmptyEnvelope delete_point_of_sale_async(tenant_id, point_of_sale_id)
Delete a point of sale

Deletes an existing point of sale by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**point_of_sale_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_point_of_sale_async

> models::PointOfSaleDtoEnvelope get_point_of_sale_async(tenant_id, point_of_sale_id)
Get point of sale by ID

Retrieves a single point of sale by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**point_of_sale_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PointOfSaleDtoEnvelope**](PointOfSaleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_point_of_sales_async

> models::PointOfSaleDtoListEnvelope get_point_of_sales_async(tenant_id)
Get point of sales

Retrieves a list of point of sales for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PointOfSaleDtoListEnvelope**](PointOfSaleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_point_of_sale_async

> models::EmptyEnvelope update_point_of_sale_async(tenant_id, point_of_sale_id, point_of_sale_update_dto)
Update a point of sale

Updates an existing point of sale by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**point_of_sale_id** | **uuid::Uuid** |  | [required] |
**point_of_sale_update_dto** | Option<[**PointOfSaleUpdateDto**](PointOfSaleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

