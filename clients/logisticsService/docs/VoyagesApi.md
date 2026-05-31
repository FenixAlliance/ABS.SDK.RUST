# \VoyagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancel_voyage_async**](VoyagesApi.md#cancel_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Cancel | Cancel a voyage
[**complete_voyage_async**](VoyagesApi.md#complete_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Complete | Complete a voyage
[**create_voyage_async**](VoyagesApi.md#create_voyage_async) | **POST** /api/v2/LogisticsService/Voyages | Create a voyage
[**create_voyage_port_call_async**](VoyagesApi.md#create_voyage_port_call_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls | Create a port call
[**delete_voyage_async**](VoyagesApi.md#delete_voyage_async) | **DELETE** /api/v2/LogisticsService/Voyages/{voyageId} | Delete a voyage
[**delete_voyage_port_call_async**](VoyagesApi.md#delete_voyage_port_call_async) | **DELETE** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/{portCallId} | Delete a port call
[**get_voyage_by_id_async**](VoyagesApi.md#get_voyage_by_id_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId} | Get voyage by ID
[**get_voyage_port_calls_async**](VoyagesApi.md#get_voyage_port_calls_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls | Get voyage port calls
[**get_voyage_port_calls_count_async**](VoyagesApi.md#get_voyage_port_calls_count_async) | **GET** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/Count | Get voyage port calls count
[**get_voyages_async**](VoyagesApi.md#get_voyages_async) | **GET** /api/v2/LogisticsService/Voyages | Get all voyages
[**get_voyages_count_async**](VoyagesApi.md#get_voyages_count_async) | **GET** /api/v2/LogisticsService/Voyages/Count | Get voyages count
[**start_voyage_async**](VoyagesApi.md#start_voyage_async) | **POST** /api/v2/LogisticsService/Voyages/{voyageId}/Start | Start a voyage
[**update_voyage_async**](VoyagesApi.md#update_voyage_async) | **PUT** /api/v2/LogisticsService/Voyages/{voyageId} | Update a voyage
[**update_voyage_port_call_async**](VoyagesApi.md#update_voyage_port_call_async) | **PUT** /api/v2/LogisticsService/Voyages/{voyageId}/PortCalls/{portCallId} | Update a port call



## cancel_voyage_async

> models::EmptyEnvelope cancel_voyage_async(tenant_id, voyage_id, api_version, x_api_version)
Cancel a voyage

Cancels a voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
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


## complete_voyage_async

> models::EmptyEnvelope complete_voyage_async(tenant_id, voyage_id, api_version, x_api_version)
Complete a voyage

Marks a voyage as completed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
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


## create_voyage_async

> models::EmptyEnvelope create_voyage_async(tenant_id, api_version, x_api_version, voyage_create_dto)
Create a voyage

Creates a new voyage for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**voyage_create_dto** | Option<[**VoyageCreateDto**](VoyageCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_voyage_port_call_async

> models::EmptyEnvelope create_voyage_port_call_async(tenant_id, voyage_id, api_version, x_api_version, voyage_port_call_create_dto)
Create a port call

Creates a new port call for a voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**voyage_port_call_create_dto** | Option<[**VoyagePortCallCreateDto**](VoyagePortCallCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_voyage_async

> models::EmptyEnvelope delete_voyage_async(tenant_id, voyage_id, api_version, x_api_version)
Delete a voyage

Deletes a voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
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


## delete_voyage_port_call_async

> models::EmptyEnvelope delete_voyage_port_call_async(tenant_id, voyage_id, port_call_id, api_version, x_api_version)
Delete a port call

Deletes a port call.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**port_call_id** | **uuid::Uuid** |  | [required] |
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


## get_voyage_by_id_async

> models::VoyageDtoEnvelope get_voyage_by_id_async(tenant_id, voyage_id, api_version, x_api_version)
Get voyage by ID

Retrieves a specific voyage by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::VoyageDtoEnvelope**](VoyageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_voyage_port_calls_async

> models::VoyagePortCallDtoListEnvelope get_voyage_port_calls_async(tenant_id, voyage_id, api_version, x_api_version)
Get voyage port calls

Retrieves all port calls for a specific voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::VoyagePortCallDtoListEnvelope**](VoyagePortCallDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_voyage_port_calls_count_async

> models::Int32Envelope get_voyage_port_calls_count_async(tenant_id, voyage_id, api_version, x_api_version)
Get voyage port calls count

Returns the count of port calls for a specific voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
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


## get_voyages_async

> models::VoyageDtoListEnvelope get_voyages_async(tenant_id, api_version, x_api_version)
Get all voyages

Retrieves all voyages for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::VoyageDtoListEnvelope**](VoyageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_voyages_count_async

> models::Int32Envelope get_voyages_count_async(tenant_id, api_version, x_api_version)
Get voyages count

Returns the count of voyages for the specified tenant.

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


## start_voyage_async

> models::EmptyEnvelope start_voyage_async(tenant_id, voyage_id, api_version, x_api_version)
Start a voyage

Starts a voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
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


## update_voyage_async

> models::EmptyEnvelope update_voyage_async(tenant_id, voyage_id, api_version, x_api_version, voyage_update_dto)
Update a voyage

Updates an existing voyage.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**voyage_update_dto** | Option<[**VoyageUpdateDto**](VoyageUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_voyage_port_call_async

> models::EmptyEnvelope update_voyage_port_call_async(tenant_id, voyage_id, port_call_id, api_version, x_api_version, voyage_port_call_update_dto)
Update a port call

Updates an existing port call.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**voyage_id** | **uuid::Uuid** |  | [required] |
**port_call_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**voyage_port_call_update_dto** | Option<[**VoyagePortCallUpdateDto**](VoyagePortCallUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

