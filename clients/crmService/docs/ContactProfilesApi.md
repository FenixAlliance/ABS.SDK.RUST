# \ContactProfilesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_profile_async**](ContactProfilesApi.md#create_contact_profile_async) | **POST** /api/v2/CrmService/ContactProfiles | Create a new contact profile
[**delete_contact_profile_async**](ContactProfilesApi.md#delete_contact_profile_async) | **DELETE** /api/v2/CrmService/ContactProfiles/{id} | Delete a contact profile
[**get_contact_profile_by_id_async**](ContactProfilesApi.md#get_contact_profile_by_id_async) | **GET** /api/v2/CrmService/ContactProfiles/{id} | Get contact profile by ID
[**get_contact_profiles_async**](ContactProfilesApi.md#get_contact_profiles_async) | **GET** /api/v2/CrmService/ContactProfiles | Get all contact profiles
[**get_contact_profiles_count_async**](ContactProfilesApi.md#get_contact_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Count | Get contact profiles count
[**get_partner_profiles_count_async**](ContactProfilesApi.md#get_partner_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Partners/Count | Get partner profiles count
[**get_patient_profiles_count_async**](ContactProfilesApi.md#get_patient_profiles_count_async) | **GET** /api/v2/CrmService/ContactProfiles/Patients/Count | Get patient profiles count
[**patch_contact_profile_async**](ContactProfilesApi.md#patch_contact_profile_async) | **PATCH** /api/v2/CrmService/ContactProfiles/{id} | Patch a contact profile
[**update_contact_profile_async**](ContactProfilesApi.md#update_contact_profile_async) | **PUT** /api/v2/CrmService/ContactProfiles/{id} | Update a contact profile



## create_contact_profile_async

> create_contact_profile_async(tenant_id, api_version, x_api_version, contact_profile_create_dto)
Create a new contact profile

Creates a new contact profile for the specified tenant. The ContactId must be provided in the request body.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_create_dto** | Option<[**ContactProfileCreateDto**](ContactProfileCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_profile_async

> delete_contact_profile_async(tenant_id, id, api_version, x_api_version)
Delete a contact profile

Deletes a contact profile for the specified tenant.

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


## get_contact_profile_by_id_async

> models::ContactProfileDto get_contact_profile_by_id_async(tenant_id, id, api_version, x_api_version)
Get contact profile by ID

Retrieves a specific contact profile by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactProfileDto**](ContactProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_profiles_async

> models::ContactProfileDtoListEnvelope get_contact_profiles_async(tenant_id, api_version, x_api_version, contact_profile_dto_collection_query_parameters)
Get all contact profiles

Retrieves all contact profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_dto_collection_query_parameters** | Option<[**ContactProfileDtoCollectionQueryParameters**](ContactProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ContactProfileDtoListEnvelope**](ContactProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_profiles_count_async

> models::Int32Envelope get_contact_profiles_count_async(tenant_id, api_version, x_api_version, contact_profile_dto_collection_query_parameters)
Get contact profiles count

Returns the count of contact profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_dto_collection_query_parameters** | Option<[**ContactProfileDtoCollectionQueryParameters**](ContactProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_partner_profiles_count_async

> models::Int32Envelope get_partner_profiles_count_async(tenant_id, api_version, x_api_version, contact_profile_dto_collection_query_parameters)
Get partner profiles count

Returns the count of partner contact profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_dto_collection_query_parameters** | Option<[**ContactProfileDtoCollectionQueryParameters**](ContactProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_patient_profiles_count_async

> models::Int32Envelope get_patient_profiles_count_async(tenant_id, api_version, x_api_version, contact_profile_dto_collection_query_parameters)
Get patient profiles count

Returns the count of patient contact profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_dto_collection_query_parameters** | Option<[**ContactProfileDtoCollectionQueryParameters**](ContactProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_contact_profile_async

> models::EmptyEnvelope patch_contact_profile_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a contact profile

Patch a contact profile

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


## update_contact_profile_async

> update_contact_profile_async(tenant_id, id, api_version, x_api_version, contact_profile_update_dto)
Update a contact profile

Updates an existing contact profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_profile_update_dto** | Option<[**ContactProfileUpdateDto**](ContactProfileUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

