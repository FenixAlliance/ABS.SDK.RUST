# \EmployeeAppraisalSessionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#create_employee_appraisal_session_async) | **POST** /api/v2/HrmsService/EmployeeAppraisalSessions | Create an employee appraisal session
[**delete_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#delete_employee_appraisal_session_async) | **DELETE** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Delete an employee appraisal session
[**get_employee_appraisal_session_by_id_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_session_by_id_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Get employee appraisal session by ID
[**get_employee_appraisal_sessions_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_sessions_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions | Get employee appraisal sessions
[**get_employee_appraisal_sessions_count_async**](EmployeeAppraisalSessionsApi.md#get_employee_appraisal_sessions_count_async) | **GET** /api/v2/HrmsService/EmployeeAppraisalSessions/Count | Count employee appraisal sessions
[**update_employee_appraisal_session_async**](EmployeeAppraisalSessionsApi.md#update_employee_appraisal_session_async) | **PUT** /api/v2/HrmsService/EmployeeAppraisalSessions/{sessionId} | Update an employee appraisal session



## create_employee_appraisal_session_async

> models::EmptyEnvelope create_employee_appraisal_session_async(tenant_id, api_version, x_api_version, employee_appraisal_session_create_dto)
Create an employee appraisal session

Creates a new employee appraisal session for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**employee_appraisal_session_create_dto** | Option<[**EmployeeAppraisalSessionCreateDto**](EmployeeAppraisalSessionCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_employee_appraisal_session_async

> models::EmptyEnvelope delete_employee_appraisal_session_async(tenant_id, session_id, api_version, x_api_version)
Delete an employee appraisal session

Deletes an employee appraisal session for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**session_id** | **uuid::Uuid** |  | [required] |
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


## get_employee_appraisal_session_by_id_async

> models::EmployeeAppraisalSessionDtoEnvelope get_employee_appraisal_session_by_id_async(tenant_id, session_id, api_version, x_api_version)
Get employee appraisal session by ID

Retrieves a specific employee appraisal session by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**session_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeAppraisalSessionDtoEnvelope**](EmployeeAppraisalSessionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employee_appraisal_sessions_async

> models::EmployeeAppraisalSessionDtoListEnvelope get_employee_appraisal_sessions_async(tenant_id, api_version, x_api_version)
Get employee appraisal sessions

Retrieves employee appraisal sessions for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmployeeAppraisalSessionDtoListEnvelope**](EmployeeAppraisalSessionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_employee_appraisal_sessions_count_async

> models::Int32Envelope get_employee_appraisal_sessions_count_async(tenant_id, api_version, x_api_version)
Count employee appraisal sessions

Counts employee appraisal sessions for the specified tenant.

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


## update_employee_appraisal_session_async

> models::EmptyEnvelope update_employee_appraisal_session_async(tenant_id, session_id, api_version, x_api_version, employee_appraisal_session_update_dto)
Update an employee appraisal session

Updates an existing employee appraisal session for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**session_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**employee_appraisal_session_update_dto** | Option<[**EmployeeAppraisalSessionUpdateDto**](EmployeeAppraisalSessionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

