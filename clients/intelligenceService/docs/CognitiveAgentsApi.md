# \CognitiveAgentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cognitive_agent_async**](CognitiveAgentsApi.md#create_cognitive_agent_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents | Create a new cognitive agent
[**delete_cognitive_agent_async**](CognitiveAgentsApi.md#delete_cognitive_agent_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{id} | Delete a cognitive agent
[**get_cognitive_agent_by_id_async**](CognitiveAgentsApi.md#get_cognitive_agent_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{id} | Get cognitive agent by ID
[**get_cognitive_agents_async**](CognitiveAgentsApi.md#get_cognitive_agents_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents | Get all cognitive agents
[**get_cognitive_agents_count_async**](CognitiveAgentsApi.md#get_cognitive_agents_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/Count | Get cognitive agents count
[**update_cognitive_agent_async**](CognitiveAgentsApi.md#update_cognitive_agent_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{id} | Update a cognitive agent



## create_cognitive_agent_async

> create_cognitive_agent_async(tenant_id, api_version, x_api_version, cognitive_agent_create_dto)
Create a new cognitive agent

Creates a new managed cognitive agent for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_create_dto** | Option<[**CognitiveAgentCreateDto**](CognitiveAgentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cognitive_agent_async

> delete_cognitive_agent_async(tenant_id, id, api_version, x_api_version)
Delete a cognitive agent

Deletes a managed cognitive agent for the specified tenant.

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


## get_cognitive_agent_by_id_async

> models::CognitiveAgentDtoEnvelope get_cognitive_agent_by_id_async(tenant_id, id, api_version, x_api_version)
Get cognitive agent by ID

Retrieves a specific managed cognitive agent by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveAgentDtoEnvelope**](CognitiveAgentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agents_async

> models::CognitiveAgentDtoListEnvelope get_cognitive_agents_async(tenant_id, api_version, x_api_version, cognitive_agent_dto_collection_query_parameters)
Get all cognitive agents

Retrieves all managed cognitive agents for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_dto_collection_query_parameters** | Option<[**CognitiveAgentDtoCollectionQueryParameters**](CognitiveAgentDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveAgentDtoListEnvelope**](CognitiveAgentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agents_count_async

> models::Int32Envelope get_cognitive_agents_count_async(tenant_id, api_version, x_api_version, cognitive_agent_dto_collection_query_parameters)
Get cognitive agents count

Returns the count of managed cognitive agents for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_dto_collection_query_parameters** | Option<[**CognitiveAgentDtoCollectionQueryParameters**](CognitiveAgentDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cognitive_agent_async

> update_cognitive_agent_async(tenant_id, id, api_version, x_api_version, cognitive_agent_update_dto)
Update a cognitive agent

Updates an existing managed cognitive agent for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_update_dto** | Option<[**CognitiveAgentUpdateDto**](CognitiveAgentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

