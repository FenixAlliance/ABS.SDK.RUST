# \CognitiveAgentMessagesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cognitive_agent_message_by_id_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_message_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages/{id} | Get a cognitive agent conversation message by ID
[**get_cognitive_agent_messages_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_messages_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages | Get all messages for a cognitive agent conversation
[**get_cognitive_agent_messages_count_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_messages_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages/Count | Get message count for a cognitive agent conversation



## get_cognitive_agent_message_by_id_async

> models::CognitiveAgentMessageDtoEnvelope get_cognitive_agent_message_by_id_async(tenant_id, agent_id, conversation_id, id, api_version, x_api_version)
Get a cognitive agent conversation message by ID

Retrieves a specific durable message of a conversation by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**conversation_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveAgentMessageDtoEnvelope**](CognitiveAgentMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_messages_async

> models::CognitiveAgentMessageDtoListEnvelope get_cognitive_agent_messages_async(tenant_id, agent_id, conversation_id, api_version, x_api_version, cognitive_agent_message_dto_collection_query_parameters)
Get all messages for a cognitive agent conversation

Retrieves all durable messages for the specified conversation, agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**conversation_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_message_dto_collection_query_parameters** | Option<[**CognitiveAgentMessageDtoCollectionQueryParameters**](CognitiveAgentMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveAgentMessageDtoListEnvelope**](CognitiveAgentMessageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_messages_count_async

> models::Int32Envelope get_cognitive_agent_messages_count_async(tenant_id, agent_id, conversation_id, api_version, x_api_version, cognitive_agent_message_dto_collection_query_parameters)
Get message count for a cognitive agent conversation

Returns the count of durable messages for the specified conversation, agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**conversation_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_message_dto_collection_query_parameters** | Option<[**CognitiveAgentMessageDtoCollectionQueryParameters**](CognitiveAgentMessageDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

