# \TrucksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**arrive_trip_async**](TrucksApi.md#arrive_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Arrive | Arrive a trip
[**cancel_trip_async**](TrucksApi.md#cancel_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Cancel | Cancel a trip
[**create_truck_async**](TrucksApi.md#create_truck_async) | **POST** /api/v2/LogisticsService/Trucks | Create a truck
[**create_truck_trip_async**](TrucksApi.md#create_truck_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips | Create a truck trip
[**delete_truck_async**](TrucksApi.md#delete_truck_async) | **DELETE** /api/v2/LogisticsService/Trucks/{truckId} | Delete a truck
[**delete_truck_trip_async**](TrucksApi.md#delete_truck_trip_async) | **DELETE** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId} | Delete a truck trip
[**deliver_trip_async**](TrucksApi.md#deliver_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Deliver | Deliver a trip
[**depart_trip_async**](TrucksApi.md#depart_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Depart | Depart a trip
[**dispatch_trip_async**](TrucksApi.md#dispatch_trip_async) | **POST** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId}/Dispatch | Dispatch a trip
[**get_truck_by_id_async**](TrucksApi.md#get_truck_by_id_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId} | Get truck by ID
[**get_truck_trips_async**](TrucksApi.md#get_truck_trips_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId}/Trips | Get truck trips
[**get_truck_trips_count_async**](TrucksApi.md#get_truck_trips_count_async) | **GET** /api/v2/LogisticsService/Trucks/{truckId}/Trips/Count | Get truck trips count
[**get_trucks_async**](TrucksApi.md#get_trucks_async) | **GET** /api/v2/LogisticsService/Trucks | Get all trucks
[**get_trucks_count_async**](TrucksApi.md#get_trucks_count_async) | **GET** /api/v2/LogisticsService/Trucks/Count | Get trucks count
[**update_truck_async**](TrucksApi.md#update_truck_async) | **PUT** /api/v2/LogisticsService/Trucks/{truckId} | Update a truck
[**update_truck_trip_async**](TrucksApi.md#update_truck_trip_async) | **PUT** /api/v2/LogisticsService/Trucks/{truckId}/Trips/{tripId} | Update a truck trip



## arrive_trip_async

> models::EmptyEnvelope arrive_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Arrive a trip

Marks a truck trip as arrived.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## cancel_trip_async

> models::EmptyEnvelope cancel_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Cancel a trip

Cancels a truck trip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## create_truck_async

> models::EmptyEnvelope create_truck_async(tenant_id, api_version, x_api_version, truck_create_dto)
Create a truck

Creates a new truck for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_create_dto** | Option<[**TruckCreateDto**](TruckCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_truck_trip_async

> models::EmptyEnvelope create_truck_trip_async(tenant_id, truck_id, api_version, x_api_version, truck_trip_create_dto)
Create a truck trip

Creates a new trip for a truck.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_trip_create_dto** | Option<[**TruckTripCreateDto**](TruckTripCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_truck_async

> models::EmptyEnvelope delete_truck_async(tenant_id, truck_id, api_version, x_api_version)
Delete a truck

Deletes a truck.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
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


## delete_truck_trip_async

> models::EmptyEnvelope delete_truck_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Delete a truck trip

Deletes a truck trip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## deliver_trip_async

> models::EmptyEnvelope deliver_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Deliver a trip

Marks a truck trip as delivered.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## depart_trip_async

> models::EmptyEnvelope depart_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Depart a trip

Marks a truck trip as departed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## dispatch_trip_async

> models::EmptyEnvelope dispatch_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version)
Dispatch a trip

Dispatches a truck trip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
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


## get_truck_by_id_async

> models::TruckDtoEnvelope get_truck_by_id_async(tenant_id, truck_id, api_version, x_api_version)
Get truck by ID

Retrieves a specific truck by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TruckDtoEnvelope**](TruckDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_truck_trips_async

> models::TruckTripDtoListEnvelope get_truck_trips_async(tenant_id, truck_id, api_version, x_api_version)
Get truck trips

Retrieves all trips for a specific truck.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TruckTripDtoListEnvelope**](TruckTripDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_truck_trips_count_async

> models::Int32Envelope get_truck_trips_count_async(tenant_id, truck_id, api_version, x_api_version)
Get truck trips count

Returns the count of trips for a specific truck.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
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


## get_trucks_async

> models::TruckDtoListEnvelope get_trucks_async(tenant_id, api_version, x_api_version)
Get all trucks

Retrieves all trucks for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TruckDtoListEnvelope**](TruckDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_trucks_count_async

> models::Int32Envelope get_trucks_count_async(tenant_id, api_version, x_api_version)
Get trucks count

Returns the count of trucks for the specified tenant.

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


## update_truck_async

> models::EmptyEnvelope update_truck_async(tenant_id, truck_id, api_version, x_api_version, truck_update_dto)
Update a truck

Updates an existing truck.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_update_dto** | Option<[**TruckUpdateDto**](TruckUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_truck_trip_async

> models::EmptyEnvelope update_truck_trip_async(tenant_id, truck_id, trip_id, api_version, x_api_version, truck_trip_update_dto)
Update a truck trip

Updates an existing truck trip.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**truck_id** | **uuid::Uuid** |  | [required] |
**trip_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**truck_trip_update_dto** | Option<[**TruckTripUpdateDto**](TruckTripUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

