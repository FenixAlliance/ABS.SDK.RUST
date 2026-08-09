# \ProductionPlansApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_production_plan_async**](ProductionPlansApi.md#create_production_plan_async) | **POST** /api/v2/ManufacturingService/ProductionPlans | Create a new production plan
[**delete_production_plan_async**](ProductionPlansApi.md#delete_production_plan_async) | **DELETE** /api/v2/ManufacturingService/ProductionPlans/{id} | Delete a production plan
[**get_production_plan_by_id_async**](ProductionPlansApi.md#get_production_plan_by_id_async) | **GET** /api/v2/ManufacturingService/ProductionPlans/{id} | Get production plan by ID
[**get_production_plans_async**](ProductionPlansApi.md#get_production_plans_async) | **GET** /api/v2/ManufacturingService/ProductionPlans | Get all production plans
[**get_production_plans_count_async**](ProductionPlansApi.md#get_production_plans_count_async) | **GET** /api/v2/ManufacturingService/ProductionPlans/Count | Get production plans count
[**patch_production_plan_async**](ProductionPlansApi.md#patch_production_plan_async) | **PATCH** /api/v2/ManufacturingService/ProductionPlans/{id} | Patch a production plan
[**update_production_plan_async**](ProductionPlansApi.md#update_production_plan_async) | **PUT** /api/v2/ManufacturingService/ProductionPlans/{id} | Update a production plan



## create_production_plan_async

> create_production_plan_async(tenant_id, api_version, x_api_version, production_plan_create_dto)
Create a new production plan

Creates a new production plan for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**production_plan_create_dto** | Option<[**ProductionPlanCreateDto**](ProductionPlanCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_production_plan_async

> delete_production_plan_async(tenant_id, id, api_version, x_api_version)
Delete a production plan

Deletes a production plan for the specified tenant.

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


## get_production_plan_by_id_async

> models::ProductionPlanDto get_production_plan_by_id_async(tenant_id, id, api_version, x_api_version)
Get production plan by ID

Retrieves a specific production plan by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProductionPlanDto**](ProductionPlanDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_production_plans_async

> models::ProductionPlanDtoListEnvelope get_production_plans_async(tenant_id, api_version, x_api_version, production_plan_dto_collection_query_parameters)
Get all production plans

Retrieves all production plans for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**production_plan_dto_collection_query_parameters** | Option<[**ProductionPlanDtoCollectionQueryParameters**](ProductionPlanDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ProductionPlanDtoListEnvelope**](ProductionPlanDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_production_plans_count_async

> models::Int32Envelope get_production_plans_count_async(tenant_id, api_version, x_api_version, production_plan_dto_collection_query_parameters)
Get production plans count

Returns the count of production plans for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**production_plan_dto_collection_query_parameters** | Option<[**ProductionPlanDtoCollectionQueryParameters**](ProductionPlanDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_production_plan_async

> models::EmptyEnvelope patch_production_plan_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a production plan

Patch a production plan

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_production_plan_async

> update_production_plan_async(tenant_id, id, api_version, x_api_version, production_plan_update_dto)
Update a production plan

Updates an existing production plan for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**production_plan_update_dto** | Option<[**ProductionPlanUpdateDto**](ProductionPlanUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

