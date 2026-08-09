# \SkillsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_skill_async**](SkillsApi.md#create_skill_async) | **POST** /api/v2/SocialService/Skills | Create a skill
[**delete_skill_async**](SkillsApi.md#delete_skill_async) | **DELETE** /api/v2/SocialService/Skills/{skillId} | Delete a skill
[**get_skill_by_id_async**](SkillsApi.md#get_skill_by_id_async) | **GET** /api/v2/SocialService/Skills/{skillId} | Get skill by ID
[**get_skills_async**](SkillsApi.md#get_skills_async) | **GET** /api/v2/SocialService/Skills | Get skills
[**get_skills_count_async**](SkillsApi.md#get_skills_count_async) | **GET** /api/v2/SocialService/Skills/Count | Count skills
[**patch_skill_async**](SkillsApi.md#patch_skill_async) | **PATCH** /api/v2/SocialService/Skills/{skillId} | Patch a skill
[**update_skill_async**](SkillsApi.md#update_skill_async) | **PUT** /api/v2/SocialService/Skills/{skillId} | Update a skill



## create_skill_async

> models::EmptyEnvelope create_skill_async(tenant_id, api_version, x_api_version, skill_create_dto)
Create a skill

Creates a new skill catalog entry for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**skill_create_dto** | Option<[**SkillCreateDto**](SkillCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_skill_async

> models::EmptyEnvelope delete_skill_async(tenant_id, skill_id, api_version, x_api_version)
Delete a skill

Deletes a skill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**skill_id** | **uuid::Uuid** |  | [required] |
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


## get_skill_by_id_async

> models::SkillDtoEnvelope get_skill_by_id_async(tenant_id, skill_id, api_version, x_api_version)
Get skill by ID

Retrieves a specific skill by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**skill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SkillDtoEnvelope**](SkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_skills_async

> models::SkillDtoListEnvelope get_skills_async(tenant_id, api_version, x_api_version, skill_dto_collection_query_parameters)
Get skills

Retrieves the skill catalog for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**skill_dto_collection_query_parameters** | Option<[**SkillDtoCollectionQueryParameters**](SkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::SkillDtoListEnvelope**](SkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_skills_count_async

> models::Int32Envelope get_skills_count_async(tenant_id, api_version, x_api_version, skill_dto_collection_query_parameters)
Count skills

Counts skill catalog entries for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**skill_dto_collection_query_parameters** | Option<[**SkillDtoCollectionQueryParameters**](SkillDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_skill_async

> models::EmptyEnvelope patch_skill_async(tenant_id, skill_id, api_version, x_api_version, patch_operation)
Patch a skill

Partially updates an existing skill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**skill_id** | **uuid::Uuid** |  | [required] |
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


## update_skill_async

> models::EmptyEnvelope update_skill_async(tenant_id, skill_id, api_version, x_api_version, skill_update_dto)
Update a skill

Updates an existing skill for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**skill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**skill_update_dto** | Option<[**SkillUpdateDto**](SkillUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

