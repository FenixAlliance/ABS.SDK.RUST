# \AppraisalWorkflowsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_appraisal_workflow_async**](AppraisalWorkflowsApi.md#create_appraisal_workflow_async) | **POST** /api/v2/HrmsService/AppraisalWorkflows | Create an appraisal workflow
[**delete_appraisal_workflow_async**](AppraisalWorkflowsApi.md#delete_appraisal_workflow_async) | **DELETE** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Delete an appraisal workflow
[**get_appraisal_workflow_by_id_async**](AppraisalWorkflowsApi.md#get_appraisal_workflow_by_id_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Get appraisal workflow by ID
[**get_appraisal_workflows_async**](AppraisalWorkflowsApi.md#get_appraisal_workflows_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows | Get appraisal workflows
[**get_appraisal_workflows_count_async**](AppraisalWorkflowsApi.md#get_appraisal_workflows_count_async) | **GET** /api/v2/HrmsService/AppraisalWorkflows/Count | Count appraisal workflows
[**update_appraisal_workflow_async**](AppraisalWorkflowsApi.md#update_appraisal_workflow_async) | **PUT** /api/v2/HrmsService/AppraisalWorkflows/{workflowId} | Update an appraisal workflow



## create_appraisal_workflow_async

> models::EmptyEnvelope create_appraisal_workflow_async(tenant_id, api_version, x_api_version, appraisal_workflow_create_dto)
Create an appraisal workflow

Creates a new appraisal workflow for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**appraisal_workflow_create_dto** | Option<[**AppraisalWorkflowCreateDto**](AppraisalWorkflowCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_appraisal_workflow_async

> models::EmptyEnvelope delete_appraisal_workflow_async(tenant_id, workflow_id, api_version, x_api_version)
Delete an appraisal workflow

Deletes an appraisal workflow for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**workflow_id** | **uuid::Uuid** |  | [required] |
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


## get_appraisal_workflow_by_id_async

> models::AppraisalWorkflowDtoEnvelope get_appraisal_workflow_by_id_async(tenant_id, workflow_id, api_version, x_api_version)
Get appraisal workflow by ID

Retrieves a specific appraisal workflow by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**workflow_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppraisalWorkflowDtoEnvelope**](AppraisalWorkflowDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_appraisal_workflows_async

> models::AppraisalWorkflowDtoListEnvelope get_appraisal_workflows_async(tenant_id, api_version, x_api_version)
Get appraisal workflows

Retrieves appraisal workflows for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AppraisalWorkflowDtoListEnvelope**](AppraisalWorkflowDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_appraisal_workflows_count_async

> models::Int32Envelope get_appraisal_workflows_count_async(tenant_id, api_version, x_api_version)
Count appraisal workflows

Counts appraisal workflows for the specified tenant.

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


## update_appraisal_workflow_async

> models::EmptyEnvelope update_appraisal_workflow_async(tenant_id, workflow_id, api_version, x_api_version, appraisal_workflow_update_dto)
Update an appraisal workflow

Updates an existing appraisal workflow for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**workflow_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**appraisal_workflow_update_dto** | Option<[**AppraisalWorkflowUpdateDto**](AppraisalWorkflowUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

