# \ShippingMethodsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_method_async**](ShippingMethodsApi.md#create_shipping_method_async) | **POST** /api/v2/ShipmentsService/ShippingMethods | Create a shipping method
[**delete_shipping_method_async**](ShippingMethodsApi.md#delete_shipping_method_async) | **DELETE** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Delete a shipping method
[**get_shipping_method_by_id_async**](ShippingMethodsApi.md#get_shipping_method_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Get shipping method by ID
[**get_shipping_methods_async**](ShippingMethodsApi.md#get_shipping_methods_async) | **GET** /api/v2/ShipmentsService/ShippingMethods | Get all shipping methods
[**get_shipping_methods_count_async**](ShippingMethodsApi.md#get_shipping_methods_count_async) | **GET** /api/v2/ShipmentsService/ShippingMethods/Count | Get shipping methods count
[**update_shipping_method_async**](ShippingMethodsApi.md#update_shipping_method_async) | **PUT** /api/v2/ShipmentsService/ShippingMethods/{methodId} | Update a shipping method



## create_shipping_method_async

> create_shipping_method_async(tenant_id, api_version, x_api_version, shipping_method_create_dto)
Create a shipping method

Creates a new shipping method.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_method_create_dto** | Option<[**ShippingMethodCreateDto**](ShippingMethodCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_method_async

> delete_shipping_method_async(tenant_id, method_id, api_version, x_api_version)
Delete a shipping method

Deletes a shipping method.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**method_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_method_by_id_async

> models::ShippingMethodDtoEnvelope get_shipping_method_by_id_async(tenant_id, method_id, api_version, x_api_version)
Get shipping method by ID

Retrieves a specific shipping method.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**method_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingMethodDtoEnvelope**](ShippingMethodDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_methods_async

> models::ShippingMethodDtoListEnvelope get_shipping_methods_async(tenant_id, api_version, x_api_version)
Get all shipping methods

Retrieves all shipping methods for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingMethodDtoListEnvelope**](ShippingMethodDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_methods_count_async

> models::Int32Envelope get_shipping_methods_count_async(tenant_id, api_version, x_api_version)
Get shipping methods count

Returns the count of shipping methods.

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


## update_shipping_method_async

> update_shipping_method_async(tenant_id, method_id, api_version, x_api_version, shipping_method_update_dto)
Update a shipping method

Updates an existing shipping method.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**method_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_method_update_dto** | Option<[**ShippingMethodUpdateDto**](ShippingMethodUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

