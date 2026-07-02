# \RequiredSkillsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_required_skill_async**](RequiredSkillsApi.md#create_required_skill_async) | **POST** /api/v2/HrmsService/RequiredSkills | Create a required skill
[**delete_required_skill_async**](RequiredSkillsApi.md#delete_required_skill_async) | **DELETE** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Delete a required skill
[**get_required_skill_by_id_async**](RequiredSkillsApi.md#get_required_skill_by_id_async) | **GET** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Get required skill by ID
[**get_required_skills_async**](RequiredSkillsApi.md#get_required_skills_async) | **GET** /api/v2/HrmsService/RequiredSkills | Get required skills
[**get_required_skills_count_async**](RequiredSkillsApi.md#get_required_skills_count_async) | **GET** /api/v2/HrmsService/RequiredSkills/Count | Count required skills
[**patch_required_skill_async**](RequiredSkillsApi.md#patch_required_skill_async) | **PATCH** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Patch a required skill
[**update_required_skill_async**](RequiredSkillsApi.md#update_required_skill_async) | **PUT** /api/v2/HrmsService/RequiredSkills/{requiredSkillId} | Update a required skill



## create_required_skill_async

> models::EmptyEnvelope create_required_skill_async(tenant_id, api_version, x_api_version, required_skill_record_create_dto)
Create a required skill

Creates a new required-skill record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**required_skill_record_create_dto** | Option<[**RequiredSkillRecordCreateDto**](RequiredSkillRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_required_skill_async

> models::EmptyEnvelope delete_required_skill_async(tenant_id, required_skill_id, api_version, x_api_version)
Delete a required skill

Deletes a required-skill record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**required_skill_id** | **uuid::Uuid** |  | [required] |
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


## get_required_skill_by_id_async

> models::RequiredSkillRecordDtoEnvelope get_required_skill_by_id_async(tenant_id, required_skill_id, api_version, x_api_version)
Get required skill by ID

Retrieves a specific required-skill record by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**required_skill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RequiredSkillRecordDtoEnvelope**](RequiredSkillRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_required_skills_async

> models::RequiredSkillRecordDtoListEnvelope get_required_skills_async(tenant_id, api_version, x_api_version)
Get required skills

Retrieves required-skill records for the specified tenant. Filter by `$filter=JobOfferId eq '...'` or `EmployerProfileId eq '...'`.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::RequiredSkillRecordDtoListEnvelope**](RequiredSkillRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_required_skills_count_async

> models::Int32Envelope get_required_skills_count_async(tenant_id, api_version, x_api_version)
Count required skills

Counts required-skill records for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_required_skill_async

> models::EmptyEnvelope patch_required_skill_async(tenant_id, required_skill_id, api_version, x_api_version, operation)
Patch a required skill

Partially updates an existing required-skill record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**required_skill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_required_skill_async

> models::EmptyEnvelope update_required_skill_async(tenant_id, required_skill_id, api_version, x_api_version, required_skill_record_update_dto)
Update a required skill

Updates an existing required-skill record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**required_skill_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**required_skill_record_update_dto** | Option<[**RequiredSkillRecordUpdateDto**](RequiredSkillRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

