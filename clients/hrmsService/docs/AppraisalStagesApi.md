# \AppraisalStagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_appraisal_stage_async**](AppraisalStagesApi.md#create_appraisal_stage_async) | **POST** /api/v2/HrmsService/AppraisalStages | Create an appraisal stage
[**delete_appraisal_stage_async**](AppraisalStagesApi.md#delete_appraisal_stage_async) | **DELETE** /api/v2/HrmsService/AppraisalStages/{stageId} | Delete an appraisal stage
[**get_appraisal_stage_by_id_async**](AppraisalStagesApi.md#get_appraisal_stage_by_id_async) | **GET** /api/v2/HrmsService/AppraisalStages/{stageId} | Get appraisal stage by ID
[**get_appraisal_stages_async**](AppraisalStagesApi.md#get_appraisal_stages_async) | **GET** /api/v2/HrmsService/AppraisalStages | Get appraisal stages
[**get_appraisal_stages_count_async**](AppraisalStagesApi.md#get_appraisal_stages_count_async) | **GET** /api/v2/HrmsService/AppraisalStages/Count | Count appraisal stages
[**update_appraisal_stage_async**](AppraisalStagesApi.md#update_appraisal_stage_async) | **PUT** /api/v2/HrmsService/AppraisalStages/{stageId} | Update an appraisal stage



## create_appraisal_stage_async

> models::EmptyEnvelope create_appraisal_stage_async(tenant_id, api_version, x_api_version, appraisal_stage_create_dto)
Create an appraisal stage

Creates a new appraisal stage for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**appraisal_stage_create_dto** | Option<[**AppraisalStageCreateDto**](AppraisalStageCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_appraisal_stage_async

> models::EmptyEnvelope delete_appraisal_stage_async(tenant_id, stage_id, api_version, x_api_version)
Delete an appraisal stage

Deletes an appraisal stage for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**stage_id** | **uuid::Uuid** |  | [required] |
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


## get_appraisal_stage_by_id_async

> models::AppraisalStageDtoEnvelope get_appraisal_stage_by_id_async(tenant_id, stage_id, api_version, x_api_version)
Get appraisal stage by ID

Retrieves a specific appraisal stage by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**stage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppraisalStageDtoEnvelope**](AppraisalStageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_appraisal_stages_async

> models::AppraisalStageDtoListEnvelope get_appraisal_stages_async(tenant_id, api_version, x_api_version)
Get appraisal stages

Retrieves appraisal stages for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppraisalStageDtoListEnvelope**](AppraisalStageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_appraisal_stages_count_async

> models::Int32Envelope get_appraisal_stages_count_async(tenant_id, api_version, x_api_version)
Count appraisal stages

Counts appraisal stages for the specified tenant.

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


## update_appraisal_stage_async

> models::EmptyEnvelope update_appraisal_stage_async(tenant_id, stage_id, api_version, x_api_version, appraisal_stage_update_dto)
Update an appraisal stage

Updates an existing appraisal stage for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**stage_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**appraisal_stage_update_dto** | Option<[**AppraisalStageUpdateDto**](AppraisalStageUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

