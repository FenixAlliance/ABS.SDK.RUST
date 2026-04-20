# \CourseUnitComponentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_unit_component_async**](CourseUnitComponentsApi.md#create_course_unit_component_async) | **POST** /api/v2/LearningService/CourseUnitComponents | Create a new course unit component
[**delete_course_unit_component_async**](CourseUnitComponentsApi.md#delete_course_unit_component_async) | **DELETE** /api/v2/LearningService/CourseUnitComponents/{componentId} | Delete a course unit component
[**get_course_unit_component_by_id_async**](CourseUnitComponentsApi.md#get_course_unit_component_by_id_async) | **GET** /api/v2/LearningService/CourseUnitComponents/{componentId} | Get course unit component by ID
[**get_course_unit_components_async**](CourseUnitComponentsApi.md#get_course_unit_components_async) | **GET** /api/v2/LearningService/CourseUnitComponents | Get all course unit components
[**get_course_unit_components_count_async**](CourseUnitComponentsApi.md#get_course_unit_components_count_async) | **GET** /api/v2/LearningService/CourseUnitComponents/Count | Get course unit components count
[**update_course_unit_component_async**](CourseUnitComponentsApi.md#update_course_unit_component_async) | **PUT** /api/v2/LearningService/CourseUnitComponents/{componentId} | Update a course unit component



## create_course_unit_component_async

> create_course_unit_component_async(tenant_id, api_version, x_api_version, course_unit_component_create_dto)
Create a new course unit component

Creates a new course unit component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_unit_component_create_dto** | Option<[**CourseUnitComponentCreateDto**](CourseUnitComponentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_unit_component_async

> delete_course_unit_component_async(tenant_id, component_id, api_version, x_api_version)
Delete a course unit component

Deletes a course unit component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**component_id** | **String** |  | [required] |
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


## get_course_unit_component_by_id_async

> models::CourseUnitComponentDto get_course_unit_component_by_id_async(component_id, api_version, x_api_version)
Get course unit component by ID

Retrieves a specific course unit component by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**component_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseUnitComponentDto**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_unit_components_async

> Vec<models::CourseUnitComponentDto> get_course_unit_components_async(tenant_id, api_version, x_api_version)
Get all course unit components

Retrieves all course unit components for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseUnitComponentDto>**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_unit_components_count_async

> i32 get_course_unit_components_count_async(tenant_id, api_version, x_api_version)
Get course unit components count

Returns the count of course unit components for the specified tenant.

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


## update_course_unit_component_async

> update_course_unit_component_async(tenant_id, component_id, api_version, x_api_version, course_unit_component_update_dto)
Update a course unit component

Updates an existing course unit component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**component_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_unit_component_update_dto** | Option<[**CourseUnitComponentUpdateDto**](CourseUnitComponentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

