# \VesselsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_vessel_async**](VesselsApi.md#create_vessel_async) | **POST** /api/v2/LogisticsService/Vessels | Create a vessel
[**delete_vessel_async**](VesselsApi.md#delete_vessel_async) | **DELETE** /api/v2/LogisticsService/Vessels/{vesselId} | Delete a vessel
[**get_vessel_by_id_async**](VesselsApi.md#get_vessel_by_id_async) | **GET** /api/v2/LogisticsService/Vessels/{vesselId} | Get vessel by ID
[**get_vessels_async**](VesselsApi.md#get_vessels_async) | **GET** /api/v2/LogisticsService/Vessels | Get all vessels
[**get_vessels_count_async**](VesselsApi.md#get_vessels_count_async) | **GET** /api/v2/LogisticsService/Vessels/Count | Get vessels count
[**update_vessel_async**](VesselsApi.md#update_vessel_async) | **PUT** /api/v2/LogisticsService/Vessels/{vesselId} | Update a vessel



## create_vessel_async

> models::EmptyEnvelope create_vessel_async(tenant_id, api_version, x_api_version, vessel_create_dto)
Create a vessel

Creates a new vessel for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**vessel_create_dto** | Option<[**VesselCreateDto**](VesselCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_vessel_async

> models::EmptyEnvelope delete_vessel_async(tenant_id, vessel_id, api_version, x_api_version)
Delete a vessel

Deletes a vessel.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**vessel_id** | **uuid::Uuid** |  | [required] |
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


## get_vessel_by_id_async

> models::VesselDtoEnvelope get_vessel_by_id_async(tenant_id, vessel_id, api_version, x_api_version)
Get vessel by ID

Retrieves a specific vessel by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**vessel_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::VesselDtoEnvelope**](VesselDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_vessels_async

> models::VesselDtoListEnvelope get_vessels_async(tenant_id, api_version, x_api_version)
Get all vessels

Retrieves all vessels for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::VesselDtoListEnvelope**](VesselDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_vessels_count_async

> models::Int32Envelope get_vessels_count_async(tenant_id, api_version, x_api_version)
Get vessels count

Returns the count of vessels for the specified tenant.

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


## update_vessel_async

> models::EmptyEnvelope update_vessel_async(tenant_id, vessel_id, api_version, x_api_version, vessel_update_dto)
Update a vessel

Updates an existing vessel.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**vessel_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**vessel_update_dto** | Option<[**VesselUpdateDto**](VesselUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

