# \TimeLogApprovalsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**request_project_hours_approval_async**](TimeLogApprovalsApi.md#request_project_hours_approval_async) | **POST** /api/v2/TimeTrackerService/TimeLogApprovals | Request project hours approval
[**update_project_hours_approval_approver_async**](TimeLogApprovalsApi.md#update_project_hours_approval_approver_async) | **PUT** /api/v2/TimeTrackerService/TimeLogApprovals/{approvalId}/Approver | Update approval approver
[**update_project_hours_approval_status_async**](TimeLogApprovalsApi.md#update_project_hours_approval_status_async) | **PUT** /api/v2/TimeTrackerService/TimeLogApprovals/{approvalId}/Status | Update approval status



## request_project_hours_approval_async

> request_project_hours_approval_async(tenant_id, api_version, x_api_version, project_hours_approval_create_dto)
Request project hours approval

Creates a new project hours approval request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_hours_approval_create_dto** | Option<[**ProjectHoursApprovalCreateDto**](ProjectHoursApprovalCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_hours_approval_approver_async

> update_project_hours_approval_approver_async(approval_id, tenant_id, api_version, x_api_version, project_hours_approval_approver_update_dto)
Update approval approver

Updates the approver of an existing project hours approval.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**approval_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_hours_approval_approver_update_dto** | Option<[**ProjectHoursApprovalApproverUpdateDto**](ProjectHoursApprovalApproverUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_project_hours_approval_status_async

> update_project_hours_approval_status_async(tenant_id, approval_id, api_version, x_api_version, project_hours_approval_status_update_dto)
Update approval status

Updates the status of an existing project hours approval.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**approval_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**project_hours_approval_status_update_dto** | Option<[**ProjectHoursApprovalStatusUpdateDto**](ProjectHoursApprovalStatusUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

