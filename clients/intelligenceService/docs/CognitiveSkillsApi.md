# \CognitiveSkillsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cognitive_skill_async**](CognitiveSkillsApi.md#create_cognitive_skill_async) | **POST** /api/v2/IntelligenceService/CognitiveSkills | Create a new cognitive skill
[**delete_cognitive_skill_async**](CognitiveSkillsApi.md#delete_cognitive_skill_async) | **DELETE** /api/v2/IntelligenceService/CognitiveSkills/{id} | Delete a cognitive skill
[**get_cognitive_skill_by_id_async**](CognitiveSkillsApi.md#get_cognitive_skill_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills/{id} | Get cognitive skill by ID
[**get_cognitive_skills_async**](CognitiveSkillsApi.md#get_cognitive_skills_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills | Get all cognitive skills
[**get_cognitive_skills_count_async**](CognitiveSkillsApi.md#get_cognitive_skills_count_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills/Count | Get cognitive skills count
[**update_cognitive_skill_async**](CognitiveSkillsApi.md#update_cognitive_skill_async) | **PUT** /api/v2/IntelligenceService/CognitiveSkills/{id} | Update a cognitive skill



## create_cognitive_skill_async

> create_cognitive_skill_async(tenant_id, api_version, x_api_version, cognitive_skill_create_dto)
Create a new cognitive skill

Creates a new reusable cognitive skill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_skill_create_dto** | Option<[**CognitiveSkillCreateDto**](CognitiveSkillCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cognitive_skill_async

> delete_cognitive_skill_async(tenant_id, id, api_version, x_api_version)
Delete a cognitive skill

Deletes a reusable cognitive skill for the specified tenant.

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


## get_cognitive_skill_by_id_async

> models::CognitiveSkillDtoEnvelope get_cognitive_skill_by_id_async(tenant_id, id, api_version, x_api_version)
Get cognitive skill by ID

Retrieves a specific reusable cognitive skill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CognitiveSkillDtoEnvelope**](CognitiveSkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_skills_async

> models::CognitiveSkillDtoListEnvelope get_cognitive_skills_async(tenant_id, api_version, x_api_version, cognitive_skill_dto_collection_query_parameters)
Get all cognitive skills

Retrieves all reusable cognitive skills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_skill_dto_collection_query_parameters** | Option<[**CognitiveSkillDtoCollectionQueryParameters**](CognitiveSkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CognitiveSkillDtoListEnvelope**](CognitiveSkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cognitive_skills_count_async

> models::Int32Envelope get_cognitive_skills_count_async(tenant_id, api_version, x_api_version, cognitive_skill_dto_collection_query_parameters)
Get cognitive skills count

Returns the count of reusable cognitive skills for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_skill_dto_collection_query_parameters** | Option<[**CognitiveSkillDtoCollectionQueryParameters**](CognitiveSkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cognitive_skill_async

> update_cognitive_skill_async(tenant_id, id, api_version, x_api_version, cognitive_skill_update_dto)
Update a cognitive skill

Updates an existing reusable cognitive skill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**cognitive_skill_update_dto** | Option<[**CognitiveSkillUpdateDto**](CognitiveSkillUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

