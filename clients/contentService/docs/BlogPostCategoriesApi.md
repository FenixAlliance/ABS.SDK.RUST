# \BlogPostCategoriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_blog_post_categories_async**](BlogPostCategoriesApi.md#count_blog_post_categories_async) | **GET** /api/v2/ContentService/BlogPostCategories/Count | Count blog post categories
[**create_blog_post_category_async**](BlogPostCategoriesApi.md#create_blog_post_category_async) | **POST** /api/v2/ContentService/BlogPostCategories | Create a blog post category
[**delete_blog_post_category_async**](BlogPostCategoriesApi.md#delete_blog_post_category_async) | **DELETE** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Delete a blog post category
[**get_blog_post_categories_async**](BlogPostCategoriesApi.md#get_blog_post_categories_async) | **GET** /api/v2/ContentService/BlogPostCategories | Get blog post categories
[**get_blog_post_category_by_id_async**](BlogPostCategoriesApi.md#get_blog_post_category_by_id_async) | **GET** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Get blog post category by ID
[**update_blog_post_category_async**](BlogPostCategoriesApi.md#update_blog_post_category_async) | **PUT** /api/v2/ContentService/BlogPostCategories/{blogPostCategoryId} | Update a blog post category



## count_blog_post_categories_async

> models::Int32Envelope count_blog_post_categories_async(tenant_id, api_version, x_api_version)
Count blog post categories

Counts all blog post categories for the specified tenant.

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


## create_blog_post_category_async

> models::EmptyEnvelope create_blog_post_category_async(tenant_id, api_version, x_api_version, blog_post_category_create_dto)
Create a blog post category

Creates a new blog post category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blog_post_category_create_dto** | Option<[**BlogPostCategoryCreateDto**](BlogPostCategoryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_blog_post_category_async

> models::EmptyEnvelope delete_blog_post_category_async(tenant_id, blog_post_category_id, api_version, x_api_version)
Delete a blog post category

Deletes a blog post category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_category_id** | **uuid::Uuid** |  | [required] |
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


## get_blog_post_categories_async

> models::BlogPostCategoryDtoListEnvelope get_blog_post_categories_async(tenant_id, api_version, x_api_version)
Get blog post categories

Retrieves all blog post categories for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogPostCategoryDtoListEnvelope**](BlogPostCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blog_post_category_by_id_async

> models::BlogPostCategoryDtoEnvelope get_blog_post_category_by_id_async(tenant_id, blog_post_category_id, api_version, x_api_version)
Get blog post category by ID

Retrieves a specific blog post category by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlogPostCategoryDtoEnvelope**](BlogPostCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_blog_post_category_async

> models::EmptyEnvelope update_blog_post_category_async(tenant_id, blog_post_category_id, api_version, x_api_version, blog_post_category_update_dto)
Update a blog post category

Updates an existing blog post category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blog_post_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blog_post_category_update_dto** | Option<[**BlogPostCategoryUpdateDto**](BlogPostCategoryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

