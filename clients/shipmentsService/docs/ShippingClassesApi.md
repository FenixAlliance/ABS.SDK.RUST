# \ShippingClassesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_class_async**](ShippingClassesApi.md#create_shipping_class_async) | **POST** /api/v2/ShipmentsService/ShippingClasses | Create a shipping class
[**delete_shipping_class_async**](ShippingClassesApi.md#delete_shipping_class_async) | **DELETE** /api/v2/ShipmentsService/ShippingClasses/{classId} | Delete a shipping class
[**get_shipping_class_by_id_async**](ShippingClassesApi.md#get_shipping_class_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingClasses/{classId} | Get shipping class by ID
[**get_shipping_classes_async**](ShippingClassesApi.md#get_shipping_classes_async) | **GET** /api/v2/ShipmentsService/ShippingClasses | Get all shipping classes
[**get_shipping_classes_count_async**](ShippingClassesApi.md#get_shipping_classes_count_async) | **GET** /api/v2/ShipmentsService/ShippingClasses/Count | Get shipping classes count
[**update_shipping_class_async**](ShippingClassesApi.md#update_shipping_class_async) | **PUT** /api/v2/ShipmentsService/ShippingClasses/{classId} | Update a shipping class



## create_shipping_class_async

> create_shipping_class_async(tenant_id, api_version, x_api_version, shipping_class_create_dto)
Create a shipping class

Creates a new shipping class.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_class_create_dto** | Option<[**ShippingClassCreateDto**](ShippingClassCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_class_async

> delete_shipping_class_async(tenant_id, class_id, api_version, x_api_version)
Delete a shipping class

Deletes a shipping class.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**class_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_class_by_id_async

> models::ShippingClassDtoEnvelope get_shipping_class_by_id_async(tenant_id, class_id, api_version, x_api_version)
Get shipping class by ID

Retrieves a specific shipping class.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**class_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingClassDtoEnvelope**](ShippingClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_classes_async

> models::ShippingClassDtoListEnvelope get_shipping_classes_async(tenant_id, api_version, x_api_version)
Get all shipping classes

Retrieves all shipping classes for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingClassDtoListEnvelope**](ShippingClassDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_classes_count_async

> models::Int32Envelope get_shipping_classes_count_async(tenant_id, api_version, x_api_version)
Get shipping classes count

Returns the count of shipping classes.

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


## update_shipping_class_async

> update_shipping_class_async(tenant_id, class_id, api_version, x_api_version, shipping_class_update_dto)
Update a shipping class

Updates an existing shipping class.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**class_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_class_update_dto** | Option<[**ShippingClassUpdateDto**](ShippingClassUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

