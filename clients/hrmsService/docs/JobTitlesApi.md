# \JobTitlesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_title_async**](JobTitlesApi.md#create_job_title_async) | **POST** /api/v2/HrmsService/JobTitles | Create a job title
[**delete_job_title_async**](JobTitlesApi.md#delete_job_title_async) | **DELETE** /api/v2/HrmsService/JobTitles/{jobTitleId} | Delete a job title
[**get_job_title_by_id_async**](JobTitlesApi.md#get_job_title_by_id_async) | **GET** /api/v2/HrmsService/JobTitles/{jobTitleId} | Get job title by ID
[**get_job_titles_async**](JobTitlesApi.md#get_job_titles_async) | **GET** /api/v2/HrmsService/JobTitles | Get job titles
[**get_job_titles_count_async**](JobTitlesApi.md#get_job_titles_count_async) | **GET** /api/v2/HrmsService/JobTitles/Count | Count job titles
[**update_job_title_async**](JobTitlesApi.md#update_job_title_async) | **PUT** /api/v2/HrmsService/JobTitles/{jobTitleId} | Update a job title



## create_job_title_async

> models::EmptyEnvelope create_job_title_async(tenant_id, api_version, x_api_version, job_title_create_dto)
Create a job title

Creates a new job title for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_title_create_dto** | Option<[**JobTitleCreateDto**](JobTitleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_title_async

> models::EmptyEnvelope delete_job_title_async(tenant_id, job_title_id, api_version, x_api_version)
Delete a job title

Deletes a job title for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_title_id** | **uuid::Uuid** |  | [required] |
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


## get_job_title_by_id_async

> models::JobTitleDtoEnvelope get_job_title_by_id_async(tenant_id, job_title_id, api_version, x_api_version)
Get job title by ID

Retrieves a specific job title by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_title_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobTitleDtoEnvelope**](JobTitleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_titles_async

> models::JobTitleDtoListEnvelope get_job_titles_async(tenant_id, api_version, x_api_version)
Get job titles

Retrieves job titles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobTitleDtoListEnvelope**](JobTitleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_titles_count_async

> models::Int32Envelope get_job_titles_count_async(tenant_id, api_version, x_api_version)
Count job titles

Counts job titles for the specified tenant.

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


## update_job_title_async

> models::EmptyEnvelope update_job_title_async(tenant_id, job_title_id, api_version, x_api_version, job_title_update_dto)
Update a job title

Updates an existing job title for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_title_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_title_update_dto** | Option<[**JobTitleUpdateDto**](JobTitleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

