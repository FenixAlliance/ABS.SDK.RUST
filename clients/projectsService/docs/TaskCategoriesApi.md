# \TaskCategoriesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_tenant_task_categories_async**](TaskCategoriesApi.md#count_tenant_task_categories_async) | **GET** /api/v2/ProjectsService/TaskCategories/Count | Counts task categories
[**create_task_category_async**](TaskCategoriesApi.md#create_task_category_async) | **POST** /api/v2/ProjectsService/TaskCategories | Creates a new task category
[**delete_task_category_async**](TaskCategoriesApi.md#delete_task_category_async) | **DELETE** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Deletes a task category
[**get_task_category_by_id_async**](TaskCategoriesApi.md#get_task_category_by_id_async) | **GET** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Gets a task category by ID
[**get_task_category_task_types_async**](TaskCategoriesApi.md#get_task_category_task_types_async) | **GET** /api/v2/ProjectsService/TaskCategories/{taskCategoryId}/Types | Retrieves task types for a category
[**get_tenant_task_categories_async**](TaskCategoriesApi.md#get_tenant_task_categories_async) | **GET** /api/v2/ProjectsService/TaskCategories | Retrieves all task categories
[**update_task_category_async**](TaskCategoriesApi.md#update_task_category_async) | **PUT** /api/v2/ProjectsService/TaskCategories/{taskCategoryId} | Updates a task category



## count_tenant_task_categories_async

> models::Int32Envelope count_tenant_task_categories_async(tenant_id)
Counts task categories

Gets the count of task categories for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_task_category_async

> models::TaskCategoryDto create_task_category_async(tenant_id, task_category_create_dto)
Creates a new task category

Creates a new task category for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**task_category_create_dto** | Option<[**TaskCategoryCreateDto**](TaskCategoryCreateDto.md)> |  |  |

### Return type

[**models::TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_task_category_async

> models::TaskCategoryDto delete_task_category_async(task_category_id, tenant_id)
Deletes a task category

Deletes the specified task category.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_category_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_task_category_by_id_async

> models::TaskCategoryDto get_task_category_by_id_async(task_category_id, tenant_id)
Gets a task category by ID

Retrieves the details of a task category using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_category_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_task_category_task_types_async

> models::TaskCategoryDto get_task_category_task_types_async(task_category_id, tenant_id)
Retrieves task types for a category

Gets all task types belonging to the specified task category.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_category_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_task_categories_async

> models::TaskCategoryDtoListEnvelope get_tenant_task_categories_async(tenant_id)
Retrieves all task categories

Gets all task categories for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::TaskCategoryDtoListEnvelope**](TaskCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_task_category_async

> models::TaskCategoryDto update_task_category_async(task_category_id, tenant_id, task_category_update_dto)
Updates a task category

Updates the specified task category.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**task_category_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**task_category_update_dto** | Option<[**TaskCategoryUpdateDto**](TaskCategoryUpdateDto.md)> |  |  |

### Return type

[**models::TaskCategoryDto**](TaskCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

