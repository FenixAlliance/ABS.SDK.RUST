# \LeaveApplicationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_leave_application_async**](LeaveApplicationsApi.md#create_leave_application_async) | **POST** /api/v2/HrmsService/LeaveApplications | Create a leave application
[**delete_leave_application_async**](LeaveApplicationsApi.md#delete_leave_application_async) | **DELETE** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Delete a leave application
[**get_leave_application_by_id_async**](LeaveApplicationsApi.md#get_leave_application_by_id_async) | **GET** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Get leave application by ID
[**get_leave_applications_async**](LeaveApplicationsApi.md#get_leave_applications_async) | **GET** /api/v2/HrmsService/LeaveApplications | Get leave applications
[**get_leave_applications_count_async**](LeaveApplicationsApi.md#get_leave_applications_count_async) | **GET** /api/v2/HrmsService/LeaveApplications/Count | Count leave applications
[**update_leave_application_async**](LeaveApplicationsApi.md#update_leave_application_async) | **PUT** /api/v2/HrmsService/LeaveApplications/{leaveApplicationId} | Update a leave application



## create_leave_application_async

> models::EmptyEnvelope create_leave_application_async(tenant_id, api_version, x_api_version, leave_application_create_dto)
Create a leave application

Creates a new leave application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**leave_application_create_dto** | Option<[**LeaveApplicationCreateDto**](LeaveApplicationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_leave_application_async

> models::EmptyEnvelope delete_leave_application_async(tenant_id, leave_application_id, api_version, x_api_version)
Delete a leave application

Deletes a leave application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_application_id** | **uuid::Uuid** |  | [required] |
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


## get_leave_application_by_id_async

> models::LeaveApplicationDtoEnvelope get_leave_application_by_id_async(tenant_id, leave_application_id, api_version, x_api_version)
Get leave application by ID

Retrieves a specific leave application by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LeaveApplicationDtoEnvelope**](LeaveApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_leave_applications_async

> models::LeaveApplicationDtoListEnvelope get_leave_applications_async(tenant_id, api_version, x_api_version)
Get leave applications

Retrieves leave applications for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LeaveApplicationDtoListEnvelope**](LeaveApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_leave_applications_count_async

> models::Int32Envelope get_leave_applications_count_async(tenant_id, api_version, x_api_version)
Count leave applications

Counts leave applications for the specified tenant.

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


## update_leave_application_async

> models::EmptyEnvelope update_leave_application_async(tenant_id, leave_application_id, api_version, x_api_version, leave_application_update_dto)
Update a leave application

Updates an existing leave application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**leave_application_update_dto** | Option<[**LeaveApplicationUpdateDto**](LeaveApplicationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

