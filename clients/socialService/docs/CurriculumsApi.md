# \CurriculumsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_curriculum_async**](CurriculumsApi.md#create_curriculum_async) | **POST** /api/v2/SocialService/Curriculums | Create a curriculum
[**delete_curriculum_async**](CurriculumsApi.md#delete_curriculum_async) | **DELETE** /api/v2/SocialService/Curriculums/{curriculumId} | Delete a curriculum
[**get_curriculum_async**](CurriculumsApi.md#get_curriculum_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId} | Get curriculum by ID
[**get_curriculums_async**](CurriculumsApi.md#get_curriculums_async) | **GET** /api/v2/SocialService/Curriculums | Get curricula
[**get_curriculums_count_async**](CurriculumsApi.md#get_curriculums_count_async) | **GET** /api/v2/SocialService/Curriculums/Count | Count curricula
[**patch_curriculum_async**](CurriculumsApi.md#patch_curriculum_async) | **PATCH** /api/v2/SocialService/Curriculums/{curriculumId} | Patch a curriculum
[**update_curriculum_async**](CurriculumsApi.md#update_curriculum_async) | **PUT** /api/v2/SocialService/Curriculums/{curriculumId} | Update a curriculum



## create_curriculum_async

> models::EmptyEnvelope create_curriculum_async(social_profile_id, tenant_id, api_version, x_api_version, curriculum_create_dto)
Create a curriculum

Creates a curriculum (CV) on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_create_dto** | Option<[**CurriculumCreateDto**](CurriculumCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_curriculum_async

> models::EmptyEnvelope delete_curriculum_async(social_profile_id, curriculum_id, tenant_id, api_version, x_api_version)
Delete a curriculum

Deletes a curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**curriculum_id** | **uuid::Uuid** |  | [required] |
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


## get_curriculum_async

> models::CurriculumDtoEnvelope get_curriculum_async(social_profile_id, curriculum_id, tenant_id, api_version, x_api_version)
Get curriculum by ID

Retrieves a specific curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**curriculum_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurriculumDtoEnvelope**](CurriculumDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_curriculums_async

> models::CurriculumDtoListEnvelope get_curriculums_async(social_profile_id, tenant_id, api_version, x_api_version)
Get curricula

Retrieves the curricula (CVs) authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurriculumDtoListEnvelope**](CurriculumDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_curriculums_count_async

> models::Int32Envelope get_curriculums_count_async(social_profile_id, tenant_id, api_version, x_api_version)
Count curricula

Returns the count of curricula authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## patch_curriculum_async

> models::EmptyEnvelope patch_curriculum_async(social_profile_id, curriculum_id, tenant_id, api_version, x_api_version, operation)
Patch a curriculum

Partially updates an existing curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**curriculum_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## update_curriculum_async

> models::EmptyEnvelope update_curriculum_async(social_profile_id, curriculum_id, tenant_id, api_version, x_api_version, curriculum_update_dto)
Update a curriculum

Updates an existing curriculum authored on the specified social profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**social_profile_id** | **uuid::Uuid** |  | [required] |
**curriculum_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**curriculum_update_dto** | Option<[**CurriculumUpdateDto**](CurriculumUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

