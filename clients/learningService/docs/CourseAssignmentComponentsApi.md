# \CourseAssignmentComponentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_assignment_component_async**](CourseAssignmentComponentsApi.md#create_course_assignment_component_async) | **POST** /api/v2/LearningService/CourseAssignmentComponents | Create a course assignment component
[**delete_course_assignment_component_async**](CourseAssignmentComponentsApi.md#delete_course_assignment_component_async) | **DELETE** /api/v2/LearningService/CourseAssignmentComponents/{componentId} | Delete a course assignment component
[**get_course_assignment_component_by_id_async**](CourseAssignmentComponentsApi.md#get_course_assignment_component_by_id_async) | **GET** /api/v2/LearningService/CourseAssignmentComponents/{componentId} | Get course assignment component by ID
[**get_course_assignment_components_async**](CourseAssignmentComponentsApi.md#get_course_assignment_components_async) | **GET** /api/v2/LearningService/CourseAssignmentComponents | Get all course assignment components
[**get_course_assignment_components_count_async**](CourseAssignmentComponentsApi.md#get_course_assignment_components_count_async) | **GET** /api/v2/LearningService/CourseAssignmentComponents/Count | Get course assignment components count
[**update_course_assignment_component_async**](CourseAssignmentComponentsApi.md#update_course_assignment_component_async) | **PUT** /api/v2/LearningService/CourseAssignmentComponents/{componentId} | Update a course assignment component



## create_course_assignment_component_async

> create_course_assignment_component_async(tenant_id, api_version, x_api_version, course_assignment_component_create_dto)
Create a course assignment component

Creates a new course assignment component for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_component_create_dto** | Option<[**CourseAssignmentComponentCreateDto**](CourseAssignmentComponentCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_assignment_component_async

> delete_course_assignment_component_async(tenant_id, component_id, api_version, x_api_version)
Delete a course assignment component

Deletes a course assignment component by its ID.

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


## get_course_assignment_component_by_id_async

> models::CourseAssignmentComponentDto get_course_assignment_component_by_id_async(component_id, api_version, x_api_version)
Get course assignment component by ID

Retrieves a specific course assignment component by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**component_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseAssignmentComponentDto**](CourseAssignmentComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignment_components_async

> Vec<models::CourseAssignmentComponentDto> get_course_assignment_components_async(tenant_id, api_version, x_api_version)
Get all course assignment components

Retrieves all course assignment components for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseAssignmentComponentDto>**](CourseAssignmentComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignment_components_count_async

> i32 get_course_assignment_components_count_async(tenant_id, api_version, x_api_version)
Get course assignment components count

Returns the count of course assignment components for the specified tenant.

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


## update_course_assignment_component_async

> update_course_assignment_component_async(tenant_id, component_id, api_version, x_api_version, course_assignment_component_update_dto)
Update a course assignment component

Updates an existing course assignment component.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**component_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_assignment_component_update_dto** | Option<[**CourseAssignmentComponentUpdateDto**](CourseAssignmentComponentUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

