# \ShippingLabelsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_label_async**](ShippingLabelsApi.md#create_shipping_label_async) | **POST** /api/v2/ShipmentsService/ShippingLabels | Create a shipping label
[**delete_shipping_label_async**](ShippingLabelsApi.md#delete_shipping_label_async) | **DELETE** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Delete a shipping label
[**get_shipping_label_by_id_async**](ShippingLabelsApi.md#get_shipping_label_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Get shipping label by ID
[**get_shipping_labels_async**](ShippingLabelsApi.md#get_shipping_labels_async) | **GET** /api/v2/ShipmentsService/ShippingLabels | Get all shipping labels
[**get_shipping_labels_count_async**](ShippingLabelsApi.md#get_shipping_labels_count_async) | **GET** /api/v2/ShipmentsService/ShippingLabels/Count | Get shipping labels count
[**update_shipping_label_async**](ShippingLabelsApi.md#update_shipping_label_async) | **PUT** /api/v2/ShipmentsService/ShippingLabels/{labelId} | Update a shipping label



## create_shipping_label_async

> create_shipping_label_async(tenant_id, api_version, x_api_version, shipping_label_create_dto)
Create a shipping label

Creates a new shipping label.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_label_create_dto** | Option<[**ShippingLabelCreateDto**](ShippingLabelCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_label_async

> delete_shipping_label_async(tenant_id, label_id, api_version, x_api_version)
Delete a shipping label

Deletes a shipping label.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**label_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_label_by_id_async

> models::ShippingLabelDtoEnvelope get_shipping_label_by_id_async(tenant_id, label_id, api_version, x_api_version)
Get shipping label by ID

Retrieves a specific shipping label.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**label_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingLabelDtoEnvelope**](ShippingLabelDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_labels_async

> models::ShippingLabelDtoListEnvelope get_shipping_labels_async(tenant_id, api_version, x_api_version)
Get all shipping labels

Retrieves all shipping labels for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingLabelDtoListEnvelope**](ShippingLabelDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_labels_count_async

> models::Int32Envelope get_shipping_labels_count_async(tenant_id, api_version, x_api_version)
Get shipping labels count

Returns the count of shipping labels.

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


## update_shipping_label_async

> update_shipping_label_async(tenant_id, label_id, api_version, x_api_version, shipping_label_update_dto)
Update a shipping label

Updates an existing shipping label.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**label_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_label_update_dto** | Option<[**ShippingLabelUpdateDto**](ShippingLabelUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

