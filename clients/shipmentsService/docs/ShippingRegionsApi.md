# \ShippingRegionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_region_async**](ShippingRegionsApi.md#create_shipping_region_async) | **POST** /api/v2/ShipmentsService/ShippingRegions | Create a shipping region
[**delete_shipping_region_async**](ShippingRegionsApi.md#delete_shipping_region_async) | **DELETE** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Delete a shipping region
[**get_shipping_region_by_id_async**](ShippingRegionsApi.md#get_shipping_region_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Get shipping region by ID
[**get_shipping_regions_async**](ShippingRegionsApi.md#get_shipping_regions_async) | **GET** /api/v2/ShipmentsService/ShippingRegions | Get all shipping regions
[**get_shipping_regions_count_async**](ShippingRegionsApi.md#get_shipping_regions_count_async) | **GET** /api/v2/ShipmentsService/ShippingRegions/Count | Get shipping regions count
[**update_shipping_region_async**](ShippingRegionsApi.md#update_shipping_region_async) | **PUT** /api/v2/ShipmentsService/ShippingRegions/{regionId} | Update a shipping region



## create_shipping_region_async

> create_shipping_region_async(tenant_id, api_version, x_api_version, shipping_region_create_dto)
Create a shipping region

Creates a new shipping region.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_region_create_dto** | Option<[**ShippingRegionCreateDto**](ShippingRegionCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_region_async

> delete_shipping_region_async(tenant_id, region_id, api_version, x_api_version)
Delete a shipping region

Deletes a shipping region.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**region_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_region_by_id_async

> models::ShippingRegionDtoEnvelope get_shipping_region_by_id_async(tenant_id, region_id, api_version, x_api_version)
Get shipping region by ID

Retrieves a specific shipping region.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**region_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingRegionDtoEnvelope**](ShippingRegionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_regions_async

> models::ShippingRegionDtoListEnvelope get_shipping_regions_async(tenant_id, api_version, x_api_version)
Get all shipping regions

Retrieves all shipping regions for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingRegionDtoListEnvelope**](ShippingRegionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_regions_count_async

> models::Int32Envelope get_shipping_regions_count_async(tenant_id, api_version, x_api_version)
Get shipping regions count

Returns the count of shipping regions.

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


## update_shipping_region_async

> update_shipping_region_async(tenant_id, region_id, api_version, x_api_version, shipping_region_update_dto)
Update a shipping region

Updates an existing shipping region.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**region_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_region_update_dto** | Option<[**ShippingRegionUpdateDto**](ShippingRegionUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

