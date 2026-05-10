# \ShippingCouriersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_courier_async**](ShippingCouriersApi.md#create_shipping_courier_async) | **POST** /api/v2/ShipmentsService/ShippingCouriers | Create a shipping courier
[**delete_shipping_courier_async**](ShippingCouriersApi.md#delete_shipping_courier_async) | **DELETE** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Delete a shipping courier
[**get_shipping_courier_by_id_async**](ShippingCouriersApi.md#get_shipping_courier_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Get shipping courier by ID
[**get_shipping_couriers_async**](ShippingCouriersApi.md#get_shipping_couriers_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers | Get all shipping couriers
[**get_shipping_couriers_count_async**](ShippingCouriersApi.md#get_shipping_couriers_count_async) | **GET** /api/v2/ShipmentsService/ShippingCouriers/Count | Get shipping couriers count
[**update_shipping_courier_async**](ShippingCouriersApi.md#update_shipping_courier_async) | **PUT** /api/v2/ShipmentsService/ShippingCouriers/{courierId} | Update a shipping courier



## create_shipping_courier_async

> create_shipping_courier_async(tenant_id, api_version, x_api_version, shipping_courier_create_dto)
Create a shipping courier

Creates a new shipping courier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_courier_create_dto** | Option<[**ShippingCourierCreateDto**](ShippingCourierCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_courier_async

> delete_shipping_courier_async(tenant_id, courier_id, api_version, x_api_version)
Delete a shipping courier

Deletes a shipping courier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**courier_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_courier_by_id_async

> models::ShippingCourierDtoEnvelope get_shipping_courier_by_id_async(tenant_id, courier_id, api_version, x_api_version)
Get shipping courier by ID

Retrieves a specific shipping courier by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**courier_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingCourierDtoEnvelope**](ShippingCourierDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_couriers_async

> models::ShippingCourierDtoListEnvelope get_shipping_couriers_async(tenant_id, api_version, x_api_version)
Get all shipping couriers

Retrieves all shipping couriers for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingCourierDtoListEnvelope**](ShippingCourierDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_couriers_count_async

> models::Int32Envelope get_shipping_couriers_count_async(tenant_id, api_version, x_api_version)
Get shipping couriers count

Returns the count of shipping couriers for the specified tenant.

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


## update_shipping_courier_async

> update_shipping_courier_async(tenant_id, courier_id, api_version, x_api_version, shipping_courier_update_dto)
Update a shipping courier

Updates an existing shipping courier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**courier_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_courier_update_dto** | Option<[**ShippingCourierUpdateDto**](ShippingCourierUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

