# \JobApplicantsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_applicant_async**](JobApplicantsApi.md#create_job_applicant_async) | **POST** /api/v2/HrmsService/JobApplicants | Create a job applicant
[**delete_job_applicant_async**](JobApplicantsApi.md#delete_job_applicant_async) | **DELETE** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Delete a job applicant
[**get_job_applicant_by_id_async**](JobApplicantsApi.md#get_job_applicant_by_id_async) | **GET** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Get job applicant by ID
[**get_job_applicants_async**](JobApplicantsApi.md#get_job_applicants_async) | **GET** /api/v2/HrmsService/JobApplicants | Get job applicants
[**get_job_applicants_count_async**](JobApplicantsApi.md#get_job_applicants_count_async) | **GET** /api/v2/HrmsService/JobApplicants/Count | Count job applicants
[**patch_job_applicant_async**](JobApplicantsApi.md#patch_job_applicant_async) | **PATCH** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Patch a job applicant
[**update_job_applicant_async**](JobApplicantsApi.md#update_job_applicant_async) | **PUT** /api/v2/HrmsService/JobApplicants/{jobApplicantId} | Update a job applicant



## create_job_applicant_async

> models::EmptyEnvelope create_job_applicant_async(tenant_id, api_version, x_api_version, job_applicant_profile_create_dto)
Create a job applicant

Creates a new job applicant (candidate) profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_applicant_profile_create_dto** | Option<[**JobApplicantProfileCreateDto**](JobApplicantProfileCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_applicant_async

> models::EmptyEnvelope delete_job_applicant_async(tenant_id, job_applicant_id, api_version, x_api_version)
Delete a job applicant

Deletes a job applicant (candidate) profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_applicant_id** | **uuid::Uuid** |  | [required] |
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


## get_job_applicant_by_id_async

> models::JobApplicantProfileDtoEnvelope get_job_applicant_by_id_async(tenant_id, job_applicant_id, api_version, x_api_version)
Get job applicant by ID

Retrieves a specific job applicant (candidate) profile by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_applicant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobApplicantProfileDtoEnvelope**](JobApplicantProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_applicants_async

> models::JobApplicantProfileDtoListEnvelope get_job_applicants_async(tenant_id, api_version, x_api_version, job_applicant_profile_dto_collection_query_parameters)
Get job applicants

Retrieves job applicant (candidate) profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_applicant_profile_dto_collection_query_parameters** | Option<[**JobApplicantProfileDtoCollectionQueryParameters**](JobApplicantProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::JobApplicantProfileDtoListEnvelope**](JobApplicantProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_applicants_count_async

> models::Int32Envelope get_job_applicants_count_async(tenant_id, api_version, x_api_version, job_applicant_profile_dto_collection_query_parameters)
Count job applicants

Counts job applicant profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_applicant_profile_dto_collection_query_parameters** | Option<[**JobApplicantProfileDtoCollectionQueryParameters**](JobApplicantProfileDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_job_applicant_async

> models::EmptyEnvelope patch_job_applicant_async(tenant_id, job_applicant_id, api_version, x_api_version, patch_operation)
Patch a job applicant

Partially updates an existing job applicant (candidate) profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_applicant_id** | **uuid::Uuid** |  | [required] |
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


## update_job_applicant_async

> models::EmptyEnvelope update_job_applicant_async(tenant_id, job_applicant_id, api_version, x_api_version, job_applicant_profile_update_dto)
Update a job applicant

Updates an existing job applicant (candidate) profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_applicant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_applicant_profile_update_dto** | Option<[**JobApplicantProfileUpdateDto**](JobApplicantProfileUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

