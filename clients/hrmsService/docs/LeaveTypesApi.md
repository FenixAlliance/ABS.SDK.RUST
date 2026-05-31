# \LeaveTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_leave_type_async**](LeaveTypesApi.md#create_leave_type_async) | **POST** /api/v2/HrmsService/LeaveTypes | Create a leave type
[**delete_leave_type_async**](LeaveTypesApi.md#delete_leave_type_async) | **DELETE** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Delete a leave type
[**get_leave_type_by_id_async**](LeaveTypesApi.md#get_leave_type_by_id_async) | **GET** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Get leave type by ID
[**get_leave_types_async**](LeaveTypesApi.md#get_leave_types_async) | **GET** /api/v2/HrmsService/LeaveTypes | Get leave types
[**get_leave_types_count_async**](LeaveTypesApi.md#get_leave_types_count_async) | **GET** /api/v2/HrmsService/LeaveTypes/Count | Count leave types
[**update_leave_type_async**](LeaveTypesApi.md#update_leave_type_async) | **PUT** /api/v2/HrmsService/LeaveTypes/{leaveTypeId} | Update a leave type



## create_leave_type_async

> models::EmptyEnvelope create_leave_type_async(tenant_id, api_version, x_api_version, leave_type_create_dto)
Create a leave type

Creates a new leave type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**leave_type_create_dto** | Option<[**LeaveTypeCreateDto**](LeaveTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_leave_type_async

> models::EmptyEnvelope delete_leave_type_async(tenant_id, leave_type_id, api_version, x_api_version)
Delete a leave type

Deletes a leave type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_type_id** | **uuid::Uuid** |  | [required] |
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


## get_leave_type_by_id_async

> models::LeaveTypeDtoEnvelope get_leave_type_by_id_async(tenant_id, leave_type_id, api_version, x_api_version)
Get leave type by ID

Retrieves a specific leave type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LeaveTypeDtoEnvelope**](LeaveTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_leave_types_async

> models::LeaveTypeDtoListEnvelope get_leave_types_async(tenant_id, api_version, x_api_version)
Get leave types

Retrieves leave types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LeaveTypeDtoListEnvelope**](LeaveTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_leave_types_count_async

> models::Int32Envelope get_leave_types_count_async(tenant_id, api_version, x_api_version)
Count leave types

Counts leave types for the specified tenant.

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


## update_leave_type_async

> models::EmptyEnvelope update_leave_type_async(tenant_id, leave_type_id, api_version, x_api_version, leave_type_update_dto)
Update a leave type

Updates an existing leave type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**leave_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**leave_type_update_dto** | Option<[**LeaveTypeUpdateDto**](LeaveTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

