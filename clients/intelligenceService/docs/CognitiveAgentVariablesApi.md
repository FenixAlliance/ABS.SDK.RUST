# \CognitiveAgentVariablesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#create_cognitive_agent_variable_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables | Add a variable to a cognitive agent
[**delete_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#delete_cognitive_agent_variable_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Remove a variable from a cognitive agent
[**get_cognitive_agent_variable_by_id_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variable_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Get a cognitive agent variable by ID
[**get_cognitive_agent_variables_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variables_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables | Get all variables for a cognitive agent
[**get_cognitive_agent_variables_count_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variables_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/Count | Get variable count for a cognitive agent
[**update_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#update_cognitive_agent_variable_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Update a cognitive agent variable



## create_cognitive_agent_variable_async

> create_cognitive_agent_variable_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_variable_create_dto)
Add a variable to a cognitive agent

Adds a key/value variable to the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_variable_create_dto** | Option<[**CognitiveAgentVariableCreateDto**](CognitiveAgentVariableCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cognitive_agent_variable_async

> delete_cognitive_agent_variable_async(tenant_id, agent_id, id, api_version, x_api_version)
Remove a variable from a cognitive agent

Removes a variable from the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
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


## get_cognitive_agent_variable_by_id_async

> models::CognitiveAgentVariableDtoEnvelope get_cognitive_agent_variable_by_id_async(tenant_id, agent_id, id, api_version, x_api_version)
Get a cognitive agent variable by ID

Retrieves a specific variable of a cognitive agent by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveAgentVariableDtoEnvelope**](CognitiveAgentVariableDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_variables_async

> models::CognitiveAgentVariableDtoListEnvelope get_cognitive_agent_variables_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_variable_dto_collection_query_parameters)
Get all variables for a cognitive agent

Retrieves all key/value variables for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_variable_dto_collection_query_parameters** | Option<[**CognitiveAgentVariableDtoCollectionQueryParameters**](CognitiveAgentVariableDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveAgentVariableDtoListEnvelope**](CognitiveAgentVariableDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_variables_count_async

> models::Int32Envelope get_cognitive_agent_variables_count_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_variable_dto_collection_query_parameters)
Get variable count for a cognitive agent

Returns the count of variables for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_variable_dto_collection_query_parameters** | Option<[**CognitiveAgentVariableDtoCollectionQueryParameters**](CognitiveAgentVariableDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cognitive_agent_variable_async

> update_cognitive_agent_variable_async(tenant_id, agent_id, id, api_version, x_api_version, cognitive_agent_variable_update_dto)
Update a cognitive agent variable

Updates the value of a variable for the specified agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_variable_update_dto** | Option<[**CognitiveAgentVariableUpdateDto**](CognitiveAgentVariableUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

