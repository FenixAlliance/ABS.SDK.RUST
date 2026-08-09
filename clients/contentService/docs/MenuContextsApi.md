# \MenuContextsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_menu_contexts_async**](MenuContextsApi.md#count_menu_contexts_async) | **GET** /api/v2/ContentService/MenuContexts/Count | Count menu contexts
[**create_menu_context_async**](MenuContextsApi.md#create_menu_context_async) | **POST** /api/v2/ContentService/MenuContexts | Create a menu context
[**delete_menu_context_async**](MenuContextsApi.md#delete_menu_context_async) | **DELETE** /api/v2/ContentService/MenuContexts/{menuContextId} | Delete a menu context
[**get_menu_context_by_id_async**](MenuContextsApi.md#get_menu_context_by_id_async) | **GET** /api/v2/ContentService/MenuContexts/{menuContextId} | Get menu context by ID
[**get_menu_contexts_async**](MenuContextsApi.md#get_menu_contexts_async) | **GET** /api/v2/ContentService/MenuContexts | Get menu contexts
[**update_menu_context_async**](MenuContextsApi.md#update_menu_context_async) | **PUT** /api/v2/ContentService/MenuContexts/{menuContextId} | Update a menu context



## count_menu_contexts_async

> models::Int32Envelope count_menu_contexts_async(tenant_id, api_version, x_api_version, menu_context_dto_collection_query_parameters)
Count menu contexts

Counts all menu contexts for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**menu_context_dto_collection_query_parameters** | Option<[**MenuContextDtoCollectionQueryParameters**](MenuContextDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_menu_context_async

> models::EmptyEnvelope create_menu_context_async(tenant_id, menu_context_create_dto, api_version, x_api_version)
Create a menu context

Creates a new menu context for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**menu_context_create_dto** | [**MenuContextCreateDto**](MenuContextCreateDto.md) |  | [required] |
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


## delete_menu_context_async

> models::EmptyEnvelope delete_menu_context_async(tenant_id, menu_context_id, api_version, x_api_version)
Delete a menu context

Deletes a menu context for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**menu_context_id** | **uuid::Uuid** |  | [required] |
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


## get_menu_context_by_id_async

> models::MenuContextDtoEnvelope get_menu_context_by_id_async(tenant_id, menu_context_id, api_version, x_api_version)
Get menu context by ID

Retrieves a specific menu context by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**menu_context_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MenuContextDtoEnvelope**](MenuContextDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_menu_contexts_async

> models::MenuContextDtoListEnvelope get_menu_contexts_async(tenant_id, api_version, x_api_version, menu_context_dto_collection_query_parameters)
Get menu contexts

Retrieves all menu contexts for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**menu_context_dto_collection_query_parameters** | Option<[**MenuContextDtoCollectionQueryParameters**](MenuContextDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::MenuContextDtoListEnvelope**](MenuContextDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_menu_context_async

> models::EmptyEnvelope update_menu_context_async(tenant_id, menu_context_id, menu_context_update_dto, api_version, x_api_version)
Update a menu context

Updates an existing menu context for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**menu_context_id** | **uuid::Uuid** |  | [required] |
**menu_context_update_dto** | [**MenuContextUpdateDto**](MenuContextUpdateDto.md) |  | [required] |
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

