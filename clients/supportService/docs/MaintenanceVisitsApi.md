# \MaintenanceVisitsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_maintenance_visit_async**](MaintenanceVisitsApi.md#create_maintenance_visit_async) | **POST** /api/v2/SupportService/MaintenanceVisits | Create a maintenance visit
[**delete_maintenance_visit_async**](MaintenanceVisitsApi.md#delete_maintenance_visit_async) | **DELETE** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Delete a maintenance visit
[**get_maintenance_visit_async**](MaintenanceVisitsApi.md#get_maintenance_visit_async) | **GET** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Retrieve a maintenance visit by ID
[**get_maintenance_visits_async**](MaintenanceVisitsApi.md#get_maintenance_visits_async) | **GET** /api/v2/SupportService/MaintenanceVisits | Retrieve maintenance visits
[**get_maintenance_visits_count_async**](MaintenanceVisitsApi.md#get_maintenance_visits_count_async) | **GET** /api/v2/SupportService/MaintenanceVisits/Count | Get maintenance visits count
[**update_maintenance_visit_async**](MaintenanceVisitsApi.md#update_maintenance_visit_async) | **PUT** /api/v2/SupportService/MaintenanceVisits/{maintenanceVisitId} | Update a maintenance visit



## create_maintenance_visit_async

> models::EmptyEnvelope create_maintenance_visit_async(tenant_id, api_version, x_api_version, maintenance_visit_create_dto)
Create a maintenance visit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**maintenance_visit_create_dto** | Option<[**MaintenanceVisitCreateDto**](MaintenanceVisitCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_maintenance_visit_async

> models::EmptyEnvelope delete_maintenance_visit_async(tenant_id, maintenance_visit_id, api_version, x_api_version)
Delete a maintenance visit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**maintenance_visit_id** | **uuid::Uuid** |  | [required] |
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


## get_maintenance_visit_async

> models::MaintenanceVisitDtoEnvelope get_maintenance_visit_async(tenant_id, maintenance_visit_id, api_version, x_api_version)
Retrieve a maintenance visit by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**maintenance_visit_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MaintenanceVisitDtoEnvelope**](MaintenanceVisitDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_maintenance_visits_async

> models::MaintenanceVisitDtoListEnvelope get_maintenance_visits_async(tenant_id, api_version, x_api_version)
Retrieve maintenance visits

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MaintenanceVisitDtoListEnvelope**](MaintenanceVisitDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_maintenance_visits_count_async

> models::Int32Envelope get_maintenance_visits_count_async(tenant_id, api_version, x_api_version)
Get maintenance visits count

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


## update_maintenance_visit_async

> models::EmptyEnvelope update_maintenance_visit_async(tenant_id, maintenance_visit_id, api_version, x_api_version, body)
Update a maintenance visit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**maintenance_visit_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**body** | Option<**serde_json::Value**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

