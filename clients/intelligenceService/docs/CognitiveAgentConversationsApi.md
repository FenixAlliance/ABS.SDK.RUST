# \CognitiveAgentConversationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#create_cognitive_agent_conversation_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations | Create a new cognitive agent conversation
[**delete_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#delete_cognitive_agent_conversation_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Delete a cognitive agent conversation
[**get_cognitive_agent_conversation_by_id_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversation_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Get a cognitive agent conversation by ID
[**get_cognitive_agent_conversations_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversations_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations | Get all conversations for a cognitive agent
[**get_cognitive_agent_conversations_count_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversations_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/Count | Get conversation count for a cognitive agent
[**update_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#update_cognitive_agent_conversation_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Update a cognitive agent conversation



## create_cognitive_agent_conversation_async

> create_cognitive_agent_conversation_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_conversation_create_dto)
Create a new cognitive agent conversation

Creates a new managed conversation for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_conversation_create_dto** | Option<[**CognitiveAgentConversationCreateDto**](CognitiveAgentConversationCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cognitive_agent_conversation_async

> delete_cognitive_agent_conversation_async(tenant_id, agent_id, id, api_version, x_api_version)
Delete a cognitive agent conversation

Deletes a managed conversation for the specified cognitive agent and tenant.

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


## get_cognitive_agent_conversation_by_id_async

> models::CognitiveAgentConversationDtoEnvelope get_cognitive_agent_conversation_by_id_async(tenant_id, agent_id, id, api_version, x_api_version)
Get a cognitive agent conversation by ID

Retrieves a specific managed conversation of a cognitive agent by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveAgentConversationDtoEnvelope**](CognitiveAgentConversationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_conversations_async

> models::CognitiveAgentConversationDtoListEnvelope get_cognitive_agent_conversations_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_conversation_dto_collection_query_parameters)
Get all conversations for a cognitive agent

Retrieves all managed conversations for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_conversation_dto_collection_query_parameters** | Option<[**CognitiveAgentConversationDtoCollectionQueryParameters**](CognitiveAgentConversationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveAgentConversationDtoListEnvelope**](CognitiveAgentConversationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_conversations_count_async

> models::Int32Envelope get_cognitive_agent_conversations_count_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_conversation_dto_collection_query_parameters)
Get conversation count for a cognitive agent

Returns the count of managed conversations for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_conversation_dto_collection_query_parameters** | Option<[**CognitiveAgentConversationDtoCollectionQueryParameters**](CognitiveAgentConversationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cognitive_agent_conversation_async

> update_cognitive_agent_conversation_async(tenant_id, agent_id, id, api_version, x_api_version, cognitive_agent_conversation_update_dto)
Update a cognitive agent conversation

Updates an existing managed conversation for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_conversation_update_dto** | Option<[**CognitiveAgentConversationUpdateDto**](CognitiveAgentConversationUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

