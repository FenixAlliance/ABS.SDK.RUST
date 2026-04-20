# \LocationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_location_async**](LocationsApi.md#create_location_async) | **POST** /api/v2/LocationsService/Locations | Create Location
[**create_wallet_location_async**](LocationsApi.md#create_wallet_location_async) | **POST** /api/v2/LocationsService/Locations/wallet/{walletId} | Create Wallet Location
[**delete_location_async**](LocationsApi.md#delete_location_async) | **DELETE** /api/v2/LocationsService/Locations/{locationId} | Delete Location
[**delete_wallet_location_async**](LocationsApi.md#delete_wallet_location_async) | **DELETE** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Delete Wallet Location
[**get_location_async**](LocationsApi.md#get_location_async) | **GET** /api/v2/LocationsService/Locations/{locationId} | Get Location
[**get_locations_async**](LocationsApi.md#get_locations_async) | **GET** /api/v2/LocationsService/Locations | Get Locations
[**get_locations_count_async**](LocationsApi.md#get_locations_count_async) | **GET** /api/v2/LocationsService/Locations/count | Get Locations Count
[**get_wallet_location_async**](LocationsApi.md#get_wallet_location_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Get Wallet Location
[**get_wallet_locations_async**](LocationsApi.md#get_wallet_locations_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId} | Get Wallet Locations
[**get_wallet_locations_count_async**](LocationsApi.md#get_wallet_locations_count_async) | **GET** /api/v2/LocationsService/Locations/wallet/{walletId}/count | Get Wallet Locations Count
[**update_location_async**](LocationsApi.md#update_location_async) | **PUT** /api/v2/LocationsService/Locations/{locationId} | Update Location
[**update_wallet_location_async**](LocationsApi.md#update_wallet_location_async) | **PUT** /api/v2/LocationsService/Locations/wallet/{walletId}/{locationId} | Update Wallet Location



## create_location_async

> models::EmptyEnvelope create_location_async(tenant_id, location_create_dto)
Create Location

Create a new location.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**location_create_dto** | Option<[**LocationCreateDto**](LocationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wallet_location_async

> models::EmptyEnvelope create_wallet_location_async(wallet_id, location_create_dto)
Create Wallet Location

Create a new location for a specific wallet.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_create_dto** | Option<[**LocationCreateDto**](LocationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_location_async

> models::EmptyEnvelope delete_location_async(tenant_id, location_id)
Delete Location

Delete a specific location by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_wallet_location_async

> models::EmptyEnvelope delete_wallet_location_async(wallet_id, location_id)
Delete Wallet Location

Delete a specific location of a wallet.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_location_async

> models::LocationDtoEnvelope get_location_async(tenant_id, location_id)
Get Location

Get details of a specific location by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_locations_async

> models::LocationDtoIReadOnlyListEnvelope get_locations_async(tenant_id)
Get Locations

Get all locations with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LocationDtoIReadOnlyListEnvelope**](LocationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_locations_count_async

> models::Int32Envelope get_locations_count_async(tenant_id)
Get Locations Count

Get the count of locations with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_location_async

> models::LocationDtoEnvelope get_wallet_location_async(wallet_id, location_id)
Get Wallet Location

Get a specific location of a wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_locations_async

> models::LocationDtoIReadOnlyListEnvelope get_wallet_locations_async(wallet_id)
Get Wallet Locations

Get locations for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LocationDtoIReadOnlyListEnvelope**](LocationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_locations_count_async

> models::Int32Envelope get_wallet_locations_count_async(wallet_id)
Get Wallet Locations Count

Get the count of locations for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_location_async

> models::EmptyEnvelope update_location_async(tenant_id, location_id, location_update_dto)
Update Location

Update a specific location by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |
**location_update_dto** | Option<[**LocationUpdateDto**](LocationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_wallet_location_async

> models::EmptyEnvelope update_wallet_location_async(wallet_id, location_id, location_update_dto)
Update Wallet Location

Update a specific location of a wallet.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |
**location_update_dto** | Option<[**LocationUpdateDto**](LocationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

