# \InstructorProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v2_learning_service_instructor_profiles_count_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_count_get) | **GET** /api/v2/LearningService/InstructorProfiles/Count | 
[**api_v2_learning_service_instructor_profiles_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_get) | **GET** /api/v2/LearningService/InstructorProfiles | 
[**api_v2_learning_service_instructor_profiles_instructor_profile_id_delete**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_delete) | **DELETE** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} | 
[**api_v2_learning_service_instructor_profiles_instructor_profile_id_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_get) | **GET** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} | 
[**api_v2_learning_service_instructor_profiles_instructor_profile_id_put**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_put) | **PUT** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} | 
[**api_v2_learning_service_instructor_profiles_post**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_post) | **POST** /api/v2/LearningService/InstructorProfiles | 



## api_v2_learning_service_instructor_profiles_count_get

> i32 api_v2_learning_service_instructor_profiles_count_get(tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

**i32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_instructor_profiles_get

> Vec<models::InstructorProfileDto> api_v2_learning_service_instructor_profiles_get(tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::InstructorProfileDto>**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_instructor_profiles_instructor_profile_id_delete

> api_v2_learning_service_instructor_profiles_instructor_profile_id_delete(tenant_id, instructor_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**instructor_profile_id** | **uuid::Uuid** |  | [required] |
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


## api_v2_learning_service_instructor_profiles_instructor_profile_id_get

> models::InstructorProfileDto api_v2_learning_service_instructor_profiles_instructor_profile_id_get(tenant_id, instructor_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**instructor_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InstructorProfileDto**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_instructor_profiles_instructor_profile_id_put

> api_v2_learning_service_instructor_profiles_instructor_profile_id_put(tenant_id, instructor_profile_id, api_version, x_api_version, instructor_profile_update_dto)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**instructor_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**instructor_profile_update_dto** | Option<[**InstructorProfileUpdateDto**](InstructorProfileUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_instructor_profiles_post

> api_v2_learning_service_instructor_profiles_post(tenant_id, api_version, x_api_version, instructor_profile_create_dto)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**instructor_profile_create_dto** | Option<[**InstructorProfileCreateDto**](InstructorProfileCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

