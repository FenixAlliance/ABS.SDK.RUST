# \CurriculumExperiencesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_curriculum_experience_async**](CurriculumExperiencesApi.md#create_curriculum_experience_async) | **POST** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences | Create a curriculum experience
[**delete_curriculum_experience_async**](CurriculumExperiencesApi.md#delete_curriculum_experience_async) | **DELETE** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Delete a curriculum experience
[**get_curriculum_experience_async**](CurriculumExperiencesApi.md#get_curriculum_experience_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Get curriculum experience by ID
[**get_curriculum_experiences_async**](CurriculumExperiencesApi.md#get_curriculum_experiences_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences | Get curriculum experiences
[**get_curriculum_experiences_count_async**](CurriculumExperiencesApi.md#get_curriculum_experiences_count_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/Count | Count curriculum experiences
[**patch_curriculum_experience_async**](CurriculumExperiencesApi.md#patch_curriculum_experience_async) | **PATCH** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Patch a curriculum experience
[**update_curriculum_experience_async**](CurriculumExperiencesApi.md#update_curriculum_experience_async) | **PUT** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Update a curriculum experience



## create_curriculum_experience_async

> models::EmptyEnvelope create_curriculum_experience_async(curriculum_id, social_profile_id, tenant_id, api_version, x_api_version, curriculum_experience_create_dto)
Create a curriculum experience

Adds a work-experience record to a curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_experience_create_dto** | Option<[**CurriculumExperienceCreateDto**](CurriculumExperienceCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_curriculum_experience_async

> models::EmptyEnvelope delete_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, tenant_id, api_version, x_api_version)
Delete a curriculum experience

Removes a work-experience record from a curriculum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**experience_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## get_curriculum_experience_async

> models::CurriculumExperienceDtoEnvelope get_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, tenant_id, api_version, x_api_version)
Get curriculum experience by ID

Retrieves a specific work-experience record of a curriculum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**experience_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurriculumExperienceDtoEnvelope**](CurriculumExperienceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_curriculum_experiences_async

> models::CurriculumExperienceDtoListEnvelope get_curriculum_experiences_async(curriculum_id, social_profile_id, tenant_id, api_version, x_api_version, curriculum_experience_dto_collection_query_parameters)
Get curriculum experiences

Retrieves the work-experience records of a curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_experience_dto_collection_query_parameters** | Option<[**CurriculumExperienceDtoCollectionQueryParameters**](CurriculumExperienceDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::CurriculumExperienceDtoListEnvelope**](CurriculumExperienceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_curriculum_experiences_count_async

> models::Int32Envelope get_curriculum_experiences_count_async(curriculum_id, social_profile_id, tenant_id, api_version, x_api_version, curriculum_experience_dto_collection_query_parameters)
Count curriculum experiences

Returns the count of work-experience records of a curriculum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_experience_dto_collection_query_parameters** | Option<[**CurriculumExperienceDtoCollectionQueryParameters**](CurriculumExperienceDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_curriculum_experience_async

> models::EmptyEnvelope patch_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, tenant_id, api_version, x_api_version, patch_operation)
Patch a curriculum experience

Partially updates an existing work-experience record of a curriculum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**experience_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## update_curriculum_experience_async

> models::EmptyEnvelope update_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, tenant_id, api_version, x_api_version, curriculum_experience_update_dto)
Update a curriculum experience

Updates an existing work-experience record of a curriculum.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**curriculum_id** | **uuid::Uuid** |  | [required] |
**experience_id** | **uuid::Uuid** |  | [required] |
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_experience_update_dto** | Option<[**CurriculumExperienceUpdateDto**](CurriculumExperienceUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

