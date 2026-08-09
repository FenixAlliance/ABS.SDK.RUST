# \CourseCategoriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_category_async**](CourseCategoriesApi.md#create_course_category_async) | **POST** /api/v2/LearningService/CourseCategories | Create a new course category
[**delete_course_category_async**](CourseCategoriesApi.md#delete_course_category_async) | **DELETE** /api/v2/LearningService/CourseCategories/{categoryId} | Delete a course category
[**get_course_categories_async**](CourseCategoriesApi.md#get_course_categories_async) | **GET** /api/v2/LearningService/CourseCategories | Get all course categories
[**get_course_categories_count_async**](CourseCategoriesApi.md#get_course_categories_count_async) | **GET** /api/v2/LearningService/CourseCategories/Count | Get course categories count
[**get_course_category_by_id_async**](CourseCategoriesApi.md#get_course_category_by_id_async) | **GET** /api/v2/LearningService/CourseCategories/{categoryId} | Get course category by ID
[**patch_course_category_async**](CourseCategoriesApi.md#patch_course_category_async) | **PATCH** /api/v2/LearningService/CourseCategories/{categoryId} | Patch a course category
[**update_course_category_async**](CourseCategoriesApi.md#update_course_category_async) | **PUT** /api/v2/LearningService/CourseCategories/{categoryId} | Update a course category



## create_course_category_async

> create_course_category_async(tenant_id, api_version, x_api_version, course_category_create_dto)
Create a new course category

Creates a new course category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_category_create_dto** | Option<[**CourseCategoryCreateDto**](CourseCategoryCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_category_async

> delete_course_category_async(tenant_id, category_id, api_version, x_api_version)
Delete a course category

Deletes a course category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **String** |  | [required] |
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


## get_course_categories_async

> Vec<models::CourseCategoryDto> get_course_categories_async(tenant_id, api_version, x_api_version, course_category_dto_collection_query_parameters)
Get all course categories

Retrieves all course categories for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_category_dto_collection_query_parameters** | Option<[**CourseCategoryDtoCollectionQueryParameters**](CourseCategoryDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**Vec<models::CourseCategoryDto>**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_categories_count_async

> i32 get_course_categories_count_async(tenant_id, api_version, x_api_version, course_category_dto_collection_query_parameters)
Get course categories count

Returns the count of course categories for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_category_dto_collection_query_parameters** | Option<[**CourseCategoryDtoCollectionQueryParameters**](CourseCategoryDtoCollectionQueryParameters.md)> |  |  |

### Return type

**i32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_category_by_id_async

> models::CourseCategoryDto get_course_category_by_id_async(category_id, api_version, x_api_version)
Get course category by ID

Retrieves a specific course category by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**category_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseCategoryDto**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_course_category_async

> models::EmptyEnvelope patch_course_category_async(tenant_id, category_id, api_version, x_api_version, patch_operation)
Patch a course category

Partially updates a course category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_course_category_async

> update_course_category_async(tenant_id, category_id, api_version, x_api_version, course_category_update_dto)
Update a course category

Updates an existing course category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_category_update_dto** | Option<[**CourseCategoryUpdateDto**](CourseCategoryUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

