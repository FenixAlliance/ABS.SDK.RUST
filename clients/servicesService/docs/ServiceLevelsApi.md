# \ServiceLevelsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_all_service_levels_async**](ServiceLevelsApi.md#count_all_service_levels_async) | **GET** /api/v2/ServicesService/ServiceLevels/Count | Get all service levels count
[**create_service_level_async**](ServiceLevelsApi.md#create_service_level_async) | **POST** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels | Create a service level
[**delete_service_level_async**](ServiceLevelsApi.md#delete_service_level_async) | **DELETE** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Delete a service level
[**get_all_service_levels_async**](ServiceLevelsApi.md#get_all_service_levels_async) | **GET** /api/v2/ServicesService/ServiceLevels | Get all service levels
[**get_service_level_by_id_async**](ServiceLevelsApi.md#get_service_level_by_id_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Get a service level by ID
[**get_service_levels_async**](ServiceLevelsApi.md#get_service_levels_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels | Get all service levels
[**get_service_levels_count_async**](ServiceLevelsApi.md#get_service_levels_count_async) | **GET** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/Count | Get service levels count
[**update_service_level_async**](ServiceLevelsApi.md#update_service_level_async) | **PUT** /api/v2/ServicesService/Services/{serviceId}/ServiceLevels/{serviceLevelId} | Update a service level



## count_all_service_levels_async

> models::Int32Envelope count_all_service_levels_async(tenant_id, api_version, x_api_version)
Get all service levels count

Returns the count of all service levels for the specified tenant.

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


## create_service_level_async

> models::Envelope create_service_level_async(tenant_id, service_id, api_version, x_api_version, service_level_create_dto)
Create a service level

Creates a new service level for the specified service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_create_dto** | Option<[**ServiceLevelCreateDto**](ServiceLevelCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_service_level_async

> models::Envelope delete_service_level_async(tenant_id, service_id, service_level_id, api_version, x_api_version)
Delete a service level

Deletes a service level by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
**service_level_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_service_levels_async

> models::ServiceLevelDtoIReadOnlyListEnvelope get_all_service_levels_async(tenant_id, api_version, x_api_version)
Get all service levels

Retrieves all service levels for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceLevelDtoIReadOnlyListEnvelope**](ServiceLevelDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_level_by_id_async

> models::ServiceLevelDtoEnvelope get_service_level_by_id_async(tenant_id, service_id, service_level_id, api_version, x_api_version)
Get a service level by ID

Retrieves a service level by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
**service_level_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceLevelDtoEnvelope**](ServiceLevelDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_levels_async

> models::ServiceLevelDtoIReadOnlyListEnvelope get_service_levels_async(tenant_id, service_id, api_version, x_api_version)
Get all service levels

Retrieves all service levels for the specified service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceLevelDtoIReadOnlyListEnvelope**](ServiceLevelDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_levels_count_async

> models::Int32Envelope get_service_levels_count_async(tenant_id, service_id, api_version, x_api_version)
Get service levels count

Returns the count of service levels for the specified service.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
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


## update_service_level_async

> models::Envelope update_service_level_async(tenant_id, service_id, service_level_id, api_version, x_api_version, service_level_update_dto)
Update a service level

Updates an existing service level.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_id** | **uuid::Uuid** |  | [required] |
**service_level_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_update_dto** | Option<[**ServiceLevelUpdateDto**](ServiceLevelUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

