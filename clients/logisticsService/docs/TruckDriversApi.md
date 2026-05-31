# \TruckDriversApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activate_truck_driver_async**](TruckDriversApi.md#activate_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers/{driverId}/Activate | Activate a truck driver
[**create_truck_driver_async**](TruckDriversApi.md#create_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers | Create a truck driver
[**deactivate_truck_driver_async**](TruckDriversApi.md#deactivate_truck_driver_async) | **POST** /api/v2/LogisticsService/TruckDrivers/{driverId}/Deactivate | Deactivate a truck driver
[**delete_truck_driver_async**](TruckDriversApi.md#delete_truck_driver_async) | **DELETE** /api/v2/LogisticsService/TruckDrivers/{driverId} | Delete a truck driver
[**get_truck_driver_by_id_async**](TruckDriversApi.md#get_truck_driver_by_id_async) | **GET** /api/v2/LogisticsService/TruckDrivers/{driverId} | Get truck driver by ID
[**get_truck_drivers_async**](TruckDriversApi.md#get_truck_drivers_async) | **GET** /api/v2/LogisticsService/TruckDrivers | Get all truck drivers
[**get_truck_drivers_count_async**](TruckDriversApi.md#get_truck_drivers_count_async) | **GET** /api/v2/LogisticsService/TruckDrivers/Count | Get truck drivers count
[**update_truck_driver_async**](TruckDriversApi.md#update_truck_driver_async) | **PUT** /api/v2/LogisticsService/TruckDrivers/{driverId} | Update a truck driver



## activate_truck_driver_async

> models::EmptyEnvelope activate_truck_driver_async(tenant_id, driver_id, api_version, x_api_version)
Activate a truck driver

Activates a truck driver.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**driver_id** | **uuid::Uuid** |  | [required] |
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


## create_truck_driver_async

> models::EmptyEnvelope create_truck_driver_async(tenant_id, api_version, x_api_version, truck_driver_create_dto)
Create a truck driver

Creates a new truck driver for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_driver_create_dto** | Option<[**TruckDriverCreateDto**](TruckDriverCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## deactivate_truck_driver_async

> models::EmptyEnvelope deactivate_truck_driver_async(tenant_id, driver_id, api_version, x_api_version)
Deactivate a truck driver

Deactivates a truck driver.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**driver_id** | **uuid::Uuid** |  | [required] |
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


## delete_truck_driver_async

> models::EmptyEnvelope delete_truck_driver_async(tenant_id, driver_id, api_version, x_api_version)
Delete a truck driver

Deletes a truck driver.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**driver_id** | **uuid::Uuid** |  | [required] |
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


## get_truck_driver_by_id_async

> models::TruckDriverDtoEnvelope get_truck_driver_by_id_async(tenant_id, driver_id, api_version, x_api_version)
Get truck driver by ID

Retrieves a specific truck driver by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**driver_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TruckDriverDtoEnvelope**](TruckDriverDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_truck_drivers_async

> models::TruckDriverDtoListEnvelope get_truck_drivers_async(tenant_id, api_version, x_api_version)
Get all truck drivers

Retrieves all truck drivers for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TruckDriverDtoListEnvelope**](TruckDriverDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_truck_drivers_count_async

> models::Int32Envelope get_truck_drivers_count_async(tenant_id, api_version, x_api_version)
Get truck drivers count

Returns the count of truck drivers for the specified tenant.

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


## update_truck_driver_async

> models::EmptyEnvelope update_truck_driver_async(tenant_id, driver_id, api_version, x_api_version, truck_driver_update_dto)
Update a truck driver

Updates an existing truck driver.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**driver_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_driver_update_dto** | Option<[**TruckDriverUpdateDto**](TruckDriverUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

