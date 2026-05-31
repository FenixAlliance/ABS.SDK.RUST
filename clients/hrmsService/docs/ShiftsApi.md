# \ShiftsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shift_async**](ShiftsApi.md#create_shift_async) | **POST** /api/v2/HrmsService/Shifts | Create a shift
[**delete_shift_async**](ShiftsApi.md#delete_shift_async) | **DELETE** /api/v2/HrmsService/Shifts/{shiftId} | Delete a shift
[**get_shift_by_id_async**](ShiftsApi.md#get_shift_by_id_async) | **GET** /api/v2/HrmsService/Shifts/{shiftId} | Get shift by ID
[**get_shifts_async**](ShiftsApi.md#get_shifts_async) | **GET** /api/v2/HrmsService/Shifts | Get shifts
[**get_shifts_count_async**](ShiftsApi.md#get_shifts_count_async) | **GET** /api/v2/HrmsService/Shifts/Count | Count shifts
[**update_shift_async**](ShiftsApi.md#update_shift_async) | **PUT** /api/v2/HrmsService/Shifts/{shiftId} | Update a shift



## create_shift_async

> models::EmptyEnvelope create_shift_async(tenant_id, api_version, x_api_version, shift_create_dto)
Create a shift

Creates a new shift for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shift_create_dto** | Option<[**ShiftCreateDto**](ShiftCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_shift_async

> models::EmptyEnvelope delete_shift_async(tenant_id, shift_id, api_version, x_api_version)
Delete a shift

Deletes a shift for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shift_id** | **uuid::Uuid** |  | [required] |
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


## get_shift_by_id_async

> models::ShiftDtoEnvelope get_shift_by_id_async(tenant_id, shift_id, api_version, x_api_version)
Get shift by ID

Retrieves a specific shift by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shift_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShiftDtoEnvelope**](ShiftDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shifts_async

> models::ShiftDtoListEnvelope get_shifts_async(tenant_id, api_version, x_api_version)
Get shifts

Retrieves shifts for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ShiftDtoListEnvelope**](ShiftDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_shifts_count_async

> models::Int32Envelope get_shifts_count_async(tenant_id, api_version, x_api_version)
Count shifts

Counts shifts for the specified tenant.

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


## update_shift_async

> models::EmptyEnvelope update_shift_async(tenant_id, shift_id, api_version, x_api_version, shift_update_dto)
Update a shift

Updates an existing shift for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**shift_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**shift_update_dto** | Option<[**ShiftUpdateDto**](ShiftUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

