# \StudentProfilesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_v2_learning_service_student_profiles_count_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_count_get) | **GET** /api/v2/LearningService/StudentProfiles/Count | 
[**api_v2_learning_service_student_profiles_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_get) | **GET** /api/v2/LearningService/StudentProfiles | 
[**api_v2_learning_service_student_profiles_post**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_post) | **POST** /api/v2/LearningService/StudentProfiles | 
[**api_v2_learning_service_student_profiles_student_profile_id_average_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_average_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId}/Average | 
[**api_v2_learning_service_student_profiles_student_profile_id_delete**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_delete) | **DELETE** /api/v2/LearningService/StudentProfiles/{studentProfileId} | 
[**api_v2_learning_service_student_profiles_student_profile_id_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId} | 
[**api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId}/HoursCompleted | 
[**api_v2_learning_service_student_profiles_student_profile_id_put**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_put) | **PUT** /api/v2/LearningService/StudentProfiles/{studentProfileId} | 



## api_v2_learning_service_student_profiles_count_get

> i32 api_v2_learning_service_student_profiles_count_get(tenant_id, api_version, x_api_version)


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


## api_v2_learning_service_student_profiles_get

> Vec<models::StudentProfileDto> api_v2_learning_service_student_profiles_get(tenant_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::StudentProfileDto>**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_student_profiles_post

> api_v2_learning_service_student_profiles_post(tenant_id, api_version, x_api_version, student_profile_create_dto)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**student_profile_create_dto** | Option<[**StudentProfileCreateDto**](StudentProfileCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_student_profiles_student_profile_id_average_get

> models::AverageDto api_v2_learning_service_student_profiles_student_profile_id_average_get(tenant_id, student_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AverageDto**](AverageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_student_profiles_student_profile_id_delete

> api_v2_learning_service_student_profiles_student_profile_id_delete(tenant_id, student_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
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


## api_v2_learning_service_student_profiles_student_profile_id_get

> models::StudentProfileDto api_v2_learning_service_student_profiles_student_profile_id_get(tenant_id, student_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::StudentProfileDto**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get

> models::CountDto api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get(tenant_id, student_profile_id, api_version, x_api_version)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountDto**](CountDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_v2_learning_service_student_profiles_student_profile_id_put

> api_v2_learning_service_student_profiles_student_profile_id_put(tenant_id, student_profile_id, api_version, x_api_version, student_profile_update_dto)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**student_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**student_profile_update_dto** | Option<[**StudentProfileUpdateDto**](StudentProfileUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

