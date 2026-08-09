# \JobOfferFieldsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_offer_field_async**](JobOfferFieldsApi.md#create_job_offer_field_async) | **POST** /api/v2/HrmsService/JobOfferFields | Create a job offer field
[**delete_job_offer_field_async**](JobOfferFieldsApi.md#delete_job_offer_field_async) | **DELETE** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Delete a job offer field
[**get_job_offer_field_by_id_async**](JobOfferFieldsApi.md#get_job_offer_field_by_id_async) | **GET** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Get job offer field by ID
[**get_job_offer_fields_async**](JobOfferFieldsApi.md#get_job_offer_fields_async) | **GET** /api/v2/HrmsService/JobOfferFields | Get job offer fields
[**get_job_offer_fields_count_async**](JobOfferFieldsApi.md#get_job_offer_fields_count_async) | **GET** /api/v2/HrmsService/JobOfferFields/Count | Count job offer fields
[**patch_job_offer_field_async**](JobOfferFieldsApi.md#patch_job_offer_field_async) | **PATCH** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Patch a job offer field
[**update_job_offer_field_async**](JobOfferFieldsApi.md#update_job_offer_field_async) | **PUT** /api/v2/HrmsService/JobOfferFields/{jobOfferFieldId} | Update a job offer field



## create_job_offer_field_async

> models::EmptyEnvelope create_job_offer_field_async(tenant_id, api_version, x_api_version, job_offer_field_record_create_dto)
Create a job offer field

Links a job field to a job offer for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_field_record_create_dto** | Option<[**JobOfferFieldRecordCreateDto**](JobOfferFieldRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_offer_field_async

> models::EmptyEnvelope delete_job_offer_field_async(tenant_id, job_offer_field_id, api_version, x_api_version)
Delete a job offer field

Removes a job-offer field link record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_field_id** | **uuid::Uuid** |  | [required] |
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


## get_job_offer_field_by_id_async

> models::JobOfferFieldRecordDtoEnvelope get_job_offer_field_by_id_async(tenant_id, job_offer_field_id, api_version, x_api_version)
Get job offer field by ID

Retrieves a specific job-offer field link record by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_field_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobOfferFieldRecordDtoEnvelope**](JobOfferFieldRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_offer_fields_async

> models::JobOfferFieldRecordDtoListEnvelope get_job_offer_fields_async(tenant_id, api_version, x_api_version, job_offer_field_record_dto_collection_query_parameters)
Get job offer fields

Retrieves job-offer field link records for the tenant. Filter with `$filter=JobOfferId eq '...'` or `JobFieldId eq '...'`.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_field_record_dto_collection_query_parameters** | Option<[**JobOfferFieldRecordDtoCollectionQueryParameters**](JobOfferFieldRecordDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::JobOfferFieldRecordDtoListEnvelope**](JobOfferFieldRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_offer_fields_count_async

> models::Int32Envelope get_job_offer_fields_count_async(tenant_id, api_version, x_api_version, job_offer_field_record_dto_collection_query_parameters)
Count job offer fields

Counts job-offer field link records for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_field_record_dto_collection_query_parameters** | Option<[**JobOfferFieldRecordDtoCollectionQueryParameters**](JobOfferFieldRecordDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_job_offer_field_async

> models::EmptyEnvelope patch_job_offer_field_async(tenant_id, job_offer_field_id, api_version, x_api_version, patch_operation)
Patch a job offer field

Partially updates an existing job-offer field link record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_field_id** | **uuid::Uuid** |  | [required] |
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


## update_job_offer_field_async

> models::EmptyEnvelope update_job_offer_field_async(tenant_id, job_offer_field_id, api_version, x_api_version, job_offer_field_record_update_dto)
Update a job offer field

Updates an existing job-offer field link record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_field_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_field_record_update_dto** | Option<[**JobOfferFieldRecordUpdateDto**](JobOfferFieldRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

