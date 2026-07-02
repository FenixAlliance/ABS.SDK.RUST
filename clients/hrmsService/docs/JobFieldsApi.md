# \JobFieldsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_field_async**](JobFieldsApi.md#create_job_field_async) | **POST** /api/v2/HrmsService/JobFields | Create a job field
[**delete_job_field_async**](JobFieldsApi.md#delete_job_field_async) | **DELETE** /api/v2/HrmsService/JobFields/{jobFieldId} | Delete a job field
[**get_job_field_by_id_async**](JobFieldsApi.md#get_job_field_by_id_async) | **GET** /api/v2/HrmsService/JobFields/{jobFieldId} | Get job field by ID
[**get_job_fields_async**](JobFieldsApi.md#get_job_fields_async) | **GET** /api/v2/HrmsService/JobFields | Get job fields
[**get_job_fields_count_async**](JobFieldsApi.md#get_job_fields_count_async) | **GET** /api/v2/HrmsService/JobFields/Count | Count job fields
[**patch_job_field_async**](JobFieldsApi.md#patch_job_field_async) | **PATCH** /api/v2/HrmsService/JobFields/{jobFieldId} | Patch a job field
[**update_job_field_async**](JobFieldsApi.md#update_job_field_async) | **PUT** /api/v2/HrmsService/JobFields/{jobFieldId} | Update a job field



## create_job_field_async

> models::EmptyEnvelope create_job_field_async(tenant_id, api_version, x_api_version, job_field_create_dto)
Create a job field

Creates a new job field (role domain) for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_field_create_dto** | Option<[**JobFieldCreateDto**](JobFieldCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_field_async

> models::EmptyEnvelope delete_job_field_async(tenant_id, job_field_id, api_version, x_api_version)
Delete a job field

Deletes a job field for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_field_id** | **uuid::Uuid** |  | [required] |
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


## get_job_field_by_id_async

> models::JobFieldDtoEnvelope get_job_field_by_id_async(tenant_id, job_field_id, api_version, x_api_version)
Get job field by ID

Retrieves a specific job field by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_field_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobFieldDtoEnvelope**](JobFieldDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_fields_async

> models::JobFieldDtoListEnvelope get_job_fields_async(tenant_id, api_version, x_api_version)
Get job fields

Retrieves job field (role domain) taxonomy entries for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobFieldDtoListEnvelope**](JobFieldDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_fields_count_async

> models::Int32Envelope get_job_fields_count_async(tenant_id, api_version, x_api_version)
Count job fields

Counts job field taxonomy entries for the specified tenant.

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


## patch_job_field_async

> models::EmptyEnvelope patch_job_field_async(tenant_id, job_field_id, api_version, x_api_version, operation)
Patch a job field

Partially updates an existing job field for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_field_id** | **uuid::Uuid** |  | [required] |
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


## update_job_field_async

> models::EmptyEnvelope update_job_field_async(tenant_id, job_field_id, api_version, x_api_version, job_field_update_dto)
Update a job field

Updates an existing job field for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_field_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_field_update_dto** | Option<[**JobFieldUpdateDto**](JobFieldUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

