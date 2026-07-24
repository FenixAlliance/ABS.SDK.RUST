# \WorkstationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_workstation_async**](WorkstationsApi.md#create_workstation_async) | **POST** /api/v2/ManufacturingService/Workstations | Create a new workstation
[**delete_workstation_async**](WorkstationsApi.md#delete_workstation_async) | **DELETE** /api/v2/ManufacturingService/Workstations/{id} | Delete a workstation
[**get_workstation_by_id_async**](WorkstationsApi.md#get_workstation_by_id_async) | **GET** /api/v2/ManufacturingService/Workstations/{id} | Get workstation by ID
[**get_workstations_async**](WorkstationsApi.md#get_workstations_async) | **GET** /api/v2/ManufacturingService/Workstations | Get all workstations
[**get_workstations_count_async**](WorkstationsApi.md#get_workstations_count_async) | **GET** /api/v2/ManufacturingService/Workstations/Count | Get workstations count
[**patch_workstation_async**](WorkstationsApi.md#patch_workstation_async) | **PATCH** /api/v2/ManufacturingService/Workstations/{id} | Patch a workstation
[**update_workstation_async**](WorkstationsApi.md#update_workstation_async) | **PUT** /api/v2/ManufacturingService/Workstations/{id} | Update a workstation



## create_workstation_async

> create_workstation_async(tenant_id, api_version, x_api_version, workstation_create_dto)
Create a new workstation

Creates a new workstation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**workstation_create_dto** | Option<[**WorkstationCreateDto**](WorkstationCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_workstation_async

> delete_workstation_async(tenant_id, id, api_version, x_api_version)
Delete a workstation

Deletes a workstation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_workstation_by_id_async

> models::WorkstationDto get_workstation_by_id_async(tenant_id, id, api_version, x_api_version)
Get workstation by ID

Retrieves a specific workstation by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkstationDto**](WorkstationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_workstations_async

> models::WorkstationDtoListEnvelope get_workstations_async(tenant_id, api_version, x_api_version)
Get all workstations

Retrieves all workstations for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WorkstationDtoListEnvelope**](WorkstationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_workstations_count_async

> models::Int32Envelope get_workstations_count_async(tenant_id, api_version, x_api_version)
Get workstations count

Returns the count of workstations for the specified tenant.

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


## patch_workstation_async

> models::EmptyEnvelope patch_workstation_async(tenant_id, id, api_version, x_api_version, operation)
Patch a workstation

Patch a workstation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_workstation_async

> update_workstation_async(tenant_id, id, api_version, x_api_version, workstation_update_dto)
Update a workstation

Updates an existing workstation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**workstation_update_dto** | Option<[**WorkstationUpdateDto**](WorkstationUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

