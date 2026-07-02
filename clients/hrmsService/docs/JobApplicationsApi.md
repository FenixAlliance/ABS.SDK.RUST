# \JobApplicationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**change_job_application_status_async**](JobApplicationsApi.md#change_job_application_status_async) | **POST** /api/v2/HrmsService/JobApplications/{jobApplicationId}/Status | Change job application status
[**create_job_application_async**](JobApplicationsApi.md#create_job_application_async) | **POST** /api/v2/HrmsService/JobApplications | Create a job application
[**delete_job_application_async**](JobApplicationsApi.md#delete_job_application_async) | **DELETE** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Delete a job application
[**get_job_application_by_id_async**](JobApplicationsApi.md#get_job_application_by_id_async) | **GET** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Get job application by ID
[**get_job_applications_async**](JobApplicationsApi.md#get_job_applications_async) | **GET** /api/v2/HrmsService/JobApplications | Get job applications
[**get_job_applications_count_async**](JobApplicationsApi.md#get_job_applications_count_async) | **GET** /api/v2/HrmsService/JobApplications/Count | Count job applications
[**patch_job_application_async**](JobApplicationsApi.md#patch_job_application_async) | **PATCH** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Patch a job application
[**update_job_application_async**](JobApplicationsApi.md#update_job_application_async) | **PUT** /api/v2/HrmsService/JobApplications/{jobApplicationId} | Update a job application



## change_job_application_status_async

> models::EmptyEnvelope change_job_application_status_async(tenant_id, job_application_id, status, api_version, x_api_version)
Change job application status

Transitions the application to a new funnel status (e.g. UnderReview, Interviewing, Offered, Hired, Rejected). Raises JobApplicationStatusChanged; terminal statuses are immutable.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_application_id** | **uuid::Uuid** |  | [required] |
**status** | **String** |  | [required] |
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


## create_job_application_async

> models::EmptyEnvelope create_job_application_async(tenant_id, api_version, x_api_version, job_offer_application_create_dto)
Create a job application

Records a candidate's application against one of the tenant's job offers. The targeted job offer must belong to the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_application_create_dto** | Option<[**JobOfferApplicationCreateDto**](JobOfferApplicationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_application_async

> models::EmptyEnvelope delete_job_application_async(tenant_id, job_application_id, api_version, x_api_version)
Delete a job application

Removes an application submitted against one of the tenant's job offers.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_application_id** | **uuid::Uuid** |  | [required] |
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


## get_job_application_by_id_async

> models::JobOfferApplicationDtoEnvelope get_job_application_by_id_async(tenant_id, job_application_id, api_version, x_api_version)
Get job application by ID

Retrieves a specific application submitted against one of the tenant's job offers.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobOfferApplicationDtoEnvelope**](JobOfferApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_applications_async

> models::JobOfferApplicationDtoListEnvelope get_job_applications_async(tenant_id, api_version, x_api_version)
Get job applications

Retrieves applications submitted against the tenant's job offers. Filter with `$filter=JobOfferId eq '...'` or `JobApplicantProfileId eq '...'`.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobOfferApplicationDtoListEnvelope**](JobOfferApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_applications_count_async

> models::Int32Envelope get_job_applications_count_async(tenant_id, api_version, x_api_version)
Count job applications

Counts applications submitted against the tenant's job offers.

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


## patch_job_application_async

> models::EmptyEnvelope patch_job_application_async(tenant_id, job_application_id, api_version, x_api_version, operation)
Patch a job application

Partially updates an existing application submitted against one of the tenant's job offers.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_application_id** | **uuid::Uuid** |  | [required] |
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


## update_job_application_async

> models::EmptyEnvelope update_job_application_async(tenant_id, job_application_id, api_version, x_api_version, job_offer_application_update_dto)
Update a job application

Updates an existing application submitted against one of the tenant's job offers.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_application_update_dto** | Option<[**JobOfferApplicationUpdateDto**](JobOfferApplicationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

