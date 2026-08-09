# \CognitiveAgentSkillsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#create_cognitive_agent_skill_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills | Assign a skill to a cognitive agent
[**delete_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#delete_cognitive_agent_skill_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Remove a skill assignment from a cognitive agent
[**get_cognitive_agent_skill_by_id_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skill_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Get a cognitive agent skill assignment by ID
[**get_cognitive_agent_skills_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skills_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills | Get all skill assignments for a cognitive agent
[**get_cognitive_agent_skills_count_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skills_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/Count | Get skill assignment count for a cognitive agent
[**update_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#update_cognitive_agent_skill_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Update a cognitive agent skill assignment



## create_cognitive_agent_skill_async

> create_cognitive_agent_skill_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_skill_create_dto)
Assign a skill to a cognitive agent

Assigns a reusable catalog skill to the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_skill_create_dto** | Option<[**CognitiveAgentSkillCreateDto**](CognitiveAgentSkillCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cognitive_agent_skill_async

> delete_cognitive_agent_skill_async(tenant_id, agent_id, id, api_version, x_api_version)
Remove a skill assignment from a cognitive agent

Removes a skill assignment from the specified cognitive agent and tenant.

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


## get_cognitive_agent_skill_by_id_async

> models::CognitiveAgentSkillDtoEnvelope get_cognitive_agent_skill_by_id_async(tenant_id, agent_id, id, api_version, x_api_version)
Get a cognitive agent skill assignment by ID

Retrieves a specific skill assignment of a cognitive agent by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveAgentSkillDtoEnvelope**](CognitiveAgentSkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_skills_async

> models::CognitiveAgentSkillDtoListEnvelope get_cognitive_agent_skills_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_skill_dto_collection_query_parameters)
Get all skill assignments for a cognitive agent

Retrieves all skill assignments for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_skill_dto_collection_query_parameters** | Option<[**CognitiveAgentSkillDtoCollectionQueryParameters**](CognitiveAgentSkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveAgentSkillDtoListEnvelope**](CognitiveAgentSkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_agent_skills_count_async

> models::Int32Envelope get_cognitive_agent_skills_count_async(tenant_id, agent_id, api_version, x_api_version, cognitive_agent_skill_dto_collection_query_parameters)
Get skill assignment count for a cognitive agent

Returns the count of skill assignments for the specified cognitive agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_skill_dto_collection_query_parameters** | Option<[**CognitiveAgentSkillDtoCollectionQueryParameters**](CognitiveAgentSkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cognitive_agent_skill_async

> update_cognitive_agent_skill_async(tenant_id, agent_id, id, api_version, x_api_version, cognitive_agent_skill_update_dto)
Update a cognitive agent skill assignment

Updates the per-assignment overrides of a skill assignment for the specified agent and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_agent_skill_update_dto** | Option<[**CognitiveAgentSkillUpdateDto**](CognitiveAgentSkillUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

