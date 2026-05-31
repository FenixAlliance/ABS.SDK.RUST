# \ShippingZonesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_zone_async**](ShippingZonesApi.md#create_shipping_zone_async) | **POST** /api/v2/ShipmentsService/ShippingZones | Create a shipping zone
[**delete_shipping_zone_async**](ShippingZonesApi.md#delete_shipping_zone_async) | **DELETE** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Delete a shipping zone
[**get_shipping_zone_by_id_async**](ShippingZonesApi.md#get_shipping_zone_by_id_async) | **GET** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Get shipping zone by ID
[**get_shipping_zones_async**](ShippingZonesApi.md#get_shipping_zones_async) | **GET** /api/v2/ShipmentsService/ShippingZones | Get all shipping zones
[**get_shipping_zones_count_async**](ShippingZonesApi.md#get_shipping_zones_count_async) | **GET** /api/v2/ShipmentsService/ShippingZones/Count | Get shipping zones count
[**update_shipping_zone_async**](ShippingZonesApi.md#update_shipping_zone_async) | **PUT** /api/v2/ShipmentsService/ShippingZones/{zoneId} | Update a shipping zone



## create_shipping_zone_async

> create_shipping_zone_async(tenant_id, api_version, x_api_version, shipping_zone_create_dto)
Create a shipping zone

Creates a new shipping zone.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_zone_create_dto** | Option<[**ShippingZoneCreateDto**](ShippingZoneCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shipping_zone_async

> delete_shipping_zone_async(tenant_id, zone_id, api_version, x_api_version)
Delete a shipping zone

Deletes a shipping zone.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**zone_id** | **uuid::Uuid** |  | [required] |
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


## get_shipping_zone_by_id_async

> models::ShippingZoneDtoEnvelope get_shipping_zone_by_id_async(tenant_id, zone_id, api_version, x_api_version)
Get shipping zone by ID

Retrieves a specific shipping zone.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**zone_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingZoneDtoEnvelope**](ShippingZoneDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_zones_async

> models::ShippingZoneDtoListEnvelope get_shipping_zones_async(tenant_id, api_version, x_api_version)
Get all shipping zones

Retrieves all shipping zones for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShippingZoneDtoListEnvelope**](ShippingZoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shipping_zones_count_async

> models::Int32Envelope get_shipping_zones_count_async(tenant_id, api_version, x_api_version)
Get shipping zones count

Returns the count of shipping zones.

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


## update_shipping_zone_async

> update_shipping_zone_async(tenant_id, zone_id, api_version, x_api_version, shipping_zone_update_dto)
Update a shipping zone

Updates an existing shipping zone.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**zone_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shipping_zone_update_dto** | Option<[**ShippingZoneUpdateDto**](ShippingZoneUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

