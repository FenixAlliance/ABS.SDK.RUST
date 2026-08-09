# \SigningProfilesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signing_profile_async**](SigningProfilesApi.md#create_signing_profile_async) | **POST** /api/v2/TrustService/SigningProfiles | Create a new signing profile
[**delete_signing_profile_async**](SigningProfilesApi.md#delete_signing_profile_async) | **DELETE** /api/v2/TrustService/SigningProfiles/{id} | Delete a signing profile
[**get_signing_profile_by_id_async**](SigningProfilesApi.md#get_signing_profile_by_id_async) | **GET** /api/v2/TrustService/SigningProfiles/{id} | Get signing profile by ID
[**get_signing_profiles_async**](SigningProfilesApi.md#get_signing_profiles_async) | **GET** /api/v2/TrustService/SigningProfiles | Get all signing profiles
[**get_signing_profiles_count_async**](SigningProfilesApi.md#get_signing_profiles_count_async) | **GET** /api/v2/TrustService/SigningProfiles/Count | Get signing profiles count
[**patch_signing_profile_async**](SigningProfilesApi.md#patch_signing_profile_async) | **PATCH** /api/v2/TrustService/SigningProfiles/{id} | Patch a signing profile
[**update_signing_profile_async**](SigningProfilesApi.md#update_signing_profile_async) | **PUT** /api/v2/TrustService/SigningProfiles/{id} | Update a signing profile



## create_signing_profile_async

> create_signing_profile_async(tenant_id, api_version, x_api_version, signing_profile_create_dto)
Create a new signing profile

Creates a new signing profile for the specified tenant (supports inline contact creation).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_create_dto** | Option<[**SigningProfileCreateDto**](SigningProfileCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_signing_profile_async

> delete_signing_profile_async(tenant_id, id, api_version, x_api_version)
Delete a signing profile

Deletes a signing profile for the specified tenant.

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


## get_signing_profile_by_id_async

> models::SigningProfileDto get_signing_profile_by_id_async(tenant_id, id, api_version, x_api_version)
Get signing profile by ID

Retrieves a specific signing profile by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningProfileDto**](SigningProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_profiles_async

> models::SigningProfileDtoListEnvelope get_signing_profiles_async(tenant_id, api_version, x_api_version, signing_profile_dto_collection_query_parameters)
Get all signing profiles

Retrieves all signing profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_dto_collection_query_parameters** | Option<[**SigningProfileDtoCollectionQueryParameters**](SigningProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::SigningProfileDtoListEnvelope**](SigningProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_profiles_count_async

> models::Int32Envelope get_signing_profiles_count_async(tenant_id, api_version, x_api_version, signing_profile_dto_collection_query_parameters)
Get signing profiles count

Returns the count of signing profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_dto_collection_query_parameters** | Option<[**SigningProfileDtoCollectionQueryParameters**](SigningProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_signing_profile_async

> models::EmptyEnvelope patch_signing_profile_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a signing profile

Patch a signing profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## update_signing_profile_async

> update_signing_profile_async(tenant_id, id, api_version, x_api_version, signing_profile_update_dto)
Update a signing profile

Updates an existing signing profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_update_dto** | Option<[**SigningProfileUpdateDto**](SigningProfileUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

