# \WebPageCategoriesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_web_page_category_async**](WebPageCategoriesApi.md#create_web_page_category_async) | **POST** /api/v2/ContentService/WebPageCategories | Create a web page category
[**delete_web_page_category_async**](WebPageCategoriesApi.md#delete_web_page_category_async) | **DELETE** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Delete a web page category
[**get_web_page_categories_async**](WebPageCategoriesApi.md#get_web_page_categories_async) | **GET** /api/v2/ContentService/WebPageCategories | Get web page categories
[**get_web_page_category_by_id_async**](WebPageCategoriesApi.md#get_web_page_category_by_id_async) | **GET** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Get web page category by ID
[**update_web_page_category_async**](WebPageCategoriesApi.md#update_web_page_category_async) | **PUT** /api/v2/ContentService/WebPageCategories/{webPageCategoryId} | Update a web page category



## create_web_page_category_async

> models::EmptyEnvelope create_web_page_category_async(tenant_id, api_version, x_api_version, web_page_category_create_dto)
Create a web page category

Creates a new web page category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_category_create_dto** | Option<[**WebPageCategoryCreateDto**](WebPageCategoryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_page_category_async

> models::EmptyEnvelope delete_web_page_category_async(tenant_id, web_page_category_id, api_version, x_api_version)
Delete a web page category

Deletes a web page category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_category_id** | **uuid::Uuid** |  | [required] |
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


## get_web_page_categories_async

> models::WebPageCategoryDtoListEnvelope get_web_page_categories_async(tenant_id, api_version, x_api_version)
Get web page categories

Retrieves all web page categories for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageCategoryDtoListEnvelope**](WebPageCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_page_category_by_id_async

> models::WebPageCategoryDtoEnvelope get_web_page_category_by_id_async(tenant_id, web_page_category_id, api_version, x_api_version)
Get web page category by ID

Retrieves a specific web page category by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageCategoryDtoEnvelope**](WebPageCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_web_page_category_async

> models::EmptyEnvelope update_web_page_category_async(tenant_id, web_page_category_id, api_version, x_api_version, web_page_category_update_dto)
Update a web page category

Updates an existing web page category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_category_update_dto** | Option<[**WebPageCategoryUpdateDto**](WebPageCategoryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

