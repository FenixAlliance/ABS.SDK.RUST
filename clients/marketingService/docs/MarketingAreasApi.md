# \MarketingAreasApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_marketing_area_async**](MarketingAreasApi.md#create_marketing_area_async) | **POST** /api/v2/MarketingService/MarketingAreas | Create a marketing area
[**delete_marketing_area_async**](MarketingAreasApi.md#delete_marketing_area_async) | **DELETE** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Delete a marketing area
[**get_marketing_area_by_id_async**](MarketingAreasApi.md#get_marketing_area_by_id_async) | **GET** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Get marketing area by ID
[**get_marketing_areas_async**](MarketingAreasApi.md#get_marketing_areas_async) | **GET** /api/v2/MarketingService/MarketingAreas | Get marketing areas
[**get_marketing_areas_count_async**](MarketingAreasApi.md#get_marketing_areas_count_async) | **GET** /api/v2/MarketingService/MarketingAreas/Count | Count marketing areas
[**update_marketing_area_async**](MarketingAreasApi.md#update_marketing_area_async) | **PUT** /api/v2/MarketingService/MarketingAreas/{marketingAreaId} | Update a marketing area



## create_marketing_area_async

> models::EmptyEnvelope create_marketing_area_async(tenant_id, api_version, x_api_version, marketing_area_create_dto)
Create a marketing area

Creates a new marketing area for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**marketing_area_create_dto** | Option<[**MarketingAreaCreateDto**](MarketingAreaCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_marketing_area_async

> models::EmptyEnvelope delete_marketing_area_async(tenant_id, marketing_area_id, api_version, x_api_version)
Delete a marketing area

Deletes a marketing area for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_area_id** | **uuid::Uuid** |  | [required] |
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


## get_marketing_area_by_id_async

> models::MarketingAreaDtoEnvelope get_marketing_area_by_id_async(tenant_id, marketing_area_id, api_version, x_api_version)
Get marketing area by ID

Retrieves a specific marketing area by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_area_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingAreaDtoEnvelope**](MarketingAreaDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_areas_async

> models::MarketingAreaDtoListEnvelope get_marketing_areas_async(tenant_id, api_version, x_api_version)
Get marketing areas

Retrieves marketing areas for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingAreaDtoListEnvelope**](MarketingAreaDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_areas_count_async

> models::Int32Envelope get_marketing_areas_count_async(tenant_id, api_version, x_api_version)
Count marketing areas

Counts marketing areas for the specified tenant.

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


## update_marketing_area_async

> models::EmptyEnvelope update_marketing_area_async(tenant_id, marketing_area_id, api_version, x_api_version, marketing_area_update_dto)
Update a marketing area

Updates an existing marketing area for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_area_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**marketing_area_update_dto** | Option<[**MarketingAreaUpdateDto**](MarketingAreaUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

