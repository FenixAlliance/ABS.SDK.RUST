# \WebComponentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_web_components_async**](WebComponentsApi.md#count_web_components_async) | **GET** /api/v2/ContentService/WebComponents/Count | Count web components
[**create_web_component_async**](WebComponentsApi.md#create_web_component_async) | **POST** /api/v2/ContentService/WebComponents | Create a web component
[**delete_web_component_async**](WebComponentsApi.md#delete_web_component_async) | **DELETE** /api/v2/ContentService/WebComponents/{webComponentId} | Delete a web component
[**get_web_component_by_id_async**](WebComponentsApi.md#get_web_component_by_id_async) | **GET** /api/v2/ContentService/WebComponents/{webComponentId} | Get web component by ID
[**get_web_components_async**](WebComponentsApi.md#get_web_components_async) | **GET** /api/v2/ContentService/WebComponents | Get web components
[**update_web_component_async**](WebComponentsApi.md#update_web_component_async) | **PUT** /api/v2/ContentService/WebComponents/{webComponentId} | Update a web component



## count_web_components_async

> models::Int32Envelope count_web_components_async(tenant_id, api_version, x_api_version, web_component_dto_collection_query_parameters)
Count web components

Counts all web components for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_component_dto_collection_query_parameters** | Option<[**WebComponentDtoCollectionQueryParameters**](WebComponentDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_web_component_async

> models::EmptyEnvelope create_web_component_async(tenant_id, web_component_create_dto, api_version, x_api_version)
Create a web component

Creates a new web component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_component_create_dto** | [**WebComponentCreateDto**](WebComponentCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_component_async

> models::EmptyEnvelope delete_web_component_async(tenant_id, web_component_id, api_version, x_api_version)
Delete a web component

Deletes a web component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_component_id** | **uuid::Uuid** |  | [required] |
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


## get_web_component_by_id_async

> models::WebComponentDtoEnvelope get_web_component_by_id_async(tenant_id, web_component_id, api_version, x_api_version)
Get web component by ID

Retrieves a specific web component by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_component_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebComponentDtoEnvelope**](WebComponentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_components_async

> models::WebComponentDtoListEnvelope get_web_components_async(tenant_id, api_version, x_api_version, web_component_dto_collection_query_parameters)
Get web components

Retrieves all web components for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_component_dto_collection_query_parameters** | Option<[**WebComponentDtoCollectionQueryParameters**](WebComponentDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::WebComponentDtoListEnvelope**](WebComponentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_web_component_async

> models::EmptyEnvelope update_web_component_async(tenant_id, web_component_id, web_component_update_dto, api_version, x_api_version)
Update a web component

Updates an existing web component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_component_id** | **uuid::Uuid** |  | [required] |
**web_component_update_dto** | [**WebComponentUpdateDto**](WebComponentUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

