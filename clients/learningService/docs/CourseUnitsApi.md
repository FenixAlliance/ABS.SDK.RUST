# \CourseUnitsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_unit_async**](CourseUnitsApi.md#create_course_unit_async) | **POST** /api/v2/LearningService/CourseUnits | Create a new course unit
[**delete_course_unit_async**](CourseUnitsApi.md#delete_course_unit_async) | **DELETE** /api/v2/LearningService/CourseUnits/{unitId} | Delete a course unit
[**get_course_unit_by_id_async**](CourseUnitsApi.md#get_course_unit_by_id_async) | **GET** /api/v2/LearningService/CourseUnits/{unitId} | Get course unit by ID
[**get_course_units_async**](CourseUnitsApi.md#get_course_units_async) | **GET** /api/v2/LearningService/CourseUnits | Get all course units
[**get_course_units_count_async**](CourseUnitsApi.md#get_course_units_count_async) | **GET** /api/v2/LearningService/CourseUnits/Count | Get course units count
[**update_course_unit_async**](CourseUnitsApi.md#update_course_unit_async) | **PUT** /api/v2/LearningService/CourseUnits/{unitId} | Update a course unit



## create_course_unit_async

> create_course_unit_async(tenant_id, api_version, x_api_version, course_unit_create_dto)
Create a new course unit

Creates a new course unit for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_unit_create_dto** | Option<[**CourseUnitCreateDto**](CourseUnitCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_unit_async

> delete_course_unit_async(tenant_id, unit_id, api_version, x_api_version)
Delete a course unit

Deletes a course unit for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**unit_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_unit_by_id_async

> models::CourseUnitDto get_course_unit_by_id_async(unit_id, api_version, x_api_version)
Get course unit by ID

Retrieves a specific course unit by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**unit_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseUnitDto**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_units_async

> Vec<models::CourseUnitDto> get_course_units_async(tenant_id, api_version, x_api_version)
Get all course units

Retrieves all course units for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseUnitDto>**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_units_count_async

> i32 get_course_units_count_async(tenant_id, api_version, x_api_version)
Get course units count

Returns the count of course units for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

**i32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_course_unit_async

> update_course_unit_async(tenant_id, unit_id, api_version, x_api_version, course_unit_update_dto)
Update a course unit

Updates an existing course unit for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**unit_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_unit_update_dto** | Option<[**CourseUnitUpdateDto**](CourseUnitUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

