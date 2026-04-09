# \WebPagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_web_pages_async**](WebPagesApi.md#count_web_pages_async) | **GET** /api/v2/ContentService/WebPages/Count | Count web pages
[**create_web_page_async**](WebPagesApi.md#create_web_page_async) | **POST** /api/v2/ContentService/WebPages | Create a web page
[**create_web_page_category_relation_async**](WebPagesApi.md#create_web_page_category_relation_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Categories | Create a web page category relation
[**create_web_page_tag_relation_async**](WebPagesApi.md#create_web_page_tag_relation_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Tags | Create a web page tag relation
[**delete_web_page_async**](WebPagesApi.md#delete_web_page_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId} | Delete a web page
[**get_categories_by_web_page_async**](WebPagesApi.md#get_categories_by_web_page_async) | **GET** /api/v2/ContentService/WebPages/{webPageId}/Categories | Get categories by web page
[**get_tags_by_web_page_async**](WebPagesApi.md#get_tags_by_web_page_async) | **GET** /api/v2/ContentService/WebPages/{webPageId}/Tags | Get tags by web page
[**get_web_page_by_id_async**](WebPagesApi.md#get_web_page_by_id_async) | **GET** /api/v2/ContentService/WebPages/{webPageId} | Get web page by ID
[**get_web_pages_async**](WebPagesApi.md#get_web_pages_async) | **GET** /api/v2/ContentService/WebPages | Get web pages
[**relate_web_page_to_category_async**](WebPagesApi.md#relate_web_page_to_category_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Categories/{categoryId} | Relate web page to category
[**relate_web_page_to_tag_async**](WebPagesApi.md#relate_web_page_to_tag_async) | **POST** /api/v2/ContentService/WebPages/{webPageId}/Tags/{tagId} | Relate web page to tag
[**unrelate_web_page_category_async**](WebPagesApi.md#unrelate_web_page_category_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId}/Categories/{categoryId} | Unrelate web page from category
[**unrelate_web_page_tag_async**](WebPagesApi.md#unrelate_web_page_tag_async) | **DELETE** /api/v2/ContentService/WebPages/{webPageId}/Tags/{tagId} | Unrelate web page from tag
[**update_web_page_async**](WebPagesApi.md#update_web_page_async) | **PUT** /api/v2/ContentService/WebPages/{webPageId} | Update a web page



## count_web_pages_async

> models::Int32Envelope count_web_pages_async(tenant_id, api_version, x_api_version)
Count web pages

Counts all web pages for the specified tenant.

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


## create_web_page_async

> create_web_page_async(tenant_id, api_version, x_api_version, web_page_create_dto)
Create a web page

Creates a new web page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_create_dto** | Option<[**WebPageCreateDto**](WebPageCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_web_page_category_relation_async

> create_web_page_category_relation_async(tenant_id, web_page_id, api_version, x_api_version, web_page_category_create_dto)
Create a web page category relation

Creates a new category and relates it to a web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_category_create_dto** | Option<[**WebPageCategoryCreateDto**](WebPageCategoryCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_web_page_tag_relation_async

> create_web_page_tag_relation_async(tenant_id, web_page_id, api_version, x_api_version, web_page_tag_create_dto)
Create a web page tag relation

Creates a new tag and relates it to a web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_tag_create_dto** | Option<[**WebPageTagCreateDto**](WebPageTagCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_page_async

> delete_web_page_async(tenant_id, web_page_id, api_version, x_api_version)
Delete a web page

Deletes a web page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
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


## get_categories_by_web_page_async

> models::WebPageCategoryDtoListEnvelope get_categories_by_web_page_async(web_page_id, api_version, x_api_version)
Get categories by web page

Retrieves all categories related to a specific web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**web_page_id** | **uuid::Uuid** |  | [required] |
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


## get_tags_by_web_page_async

> models::WebPageTagDtoListEnvelope get_tags_by_web_page_async(web_page_id, api_version, x_api_version)
Get tags by web page

Retrieves all tags related to a specific web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**web_page_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageTagDtoListEnvelope**](WebPageTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_page_by_id_async

> models::WebPageDtoEnvelope get_web_page_by_id_async(tenant_id, web_page_id, api_version, x_api_version)
Get web page by ID

Retrieves a specific web page by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageDtoEnvelope**](WebPageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_pages_async

> models::WebPageDtoListEnvelope get_web_pages_async(tenant_id, api_version, x_api_version)
Get web pages

Retrieves all web pages for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageDtoListEnvelope**](WebPageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_web_page_to_category_async

> relate_web_page_to_category_async(tenant_id, web_page_id, category_id, api_version, x_api_version)
Relate web page to category

Relates an existing category to a web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
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


## relate_web_page_to_tag_async

> relate_web_page_to_tag_async(tenant_id, web_page_id, tag_id, api_version, x_api_version)
Relate web page to tag

Relates an existing tag to a web page.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**tag_id** | **uuid::Uuid** |  | [required] |
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


## unrelate_web_page_category_async

> unrelate_web_page_category_async(tenant_id, web_page_id, category_id, api_version, x_api_version)
Unrelate web page from category

Removes the relationship between a web page and a category.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
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


## unrelate_web_page_tag_async

> unrelate_web_page_tag_async(tenant_id, web_page_id, tag_id, api_version, x_api_version)
Unrelate web page from tag

Removes the relationship between a web page and a tag.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**tag_id** | **uuid::Uuid** |  | [required] |
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


## update_web_page_async

> update_web_page_async(tenant_id, web_page_id, api_version, x_api_version, web_page_update_dto)
Update a web page

Updates an existing web page for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_update_dto** | Option<[**WebPageUpdateDto**](WebPageUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

