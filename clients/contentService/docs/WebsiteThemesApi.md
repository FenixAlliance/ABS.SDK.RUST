# \WebsiteThemesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_website_theme_async**](WebsiteThemesApi.md#create_website_theme_async) | **POST** /api/v2/ContentService/WebsiteThemes | Create a new website theme
[**delete_website_theme_async**](WebsiteThemesApi.md#delete_website_theme_async) | **DELETE** /api/v2/ContentService/WebsiteThemes/{id} | Delete a website theme
[**get_website_theme_by_id_async**](WebsiteThemesApi.md#get_website_theme_by_id_async) | **GET** /api/v2/ContentService/WebsiteThemes/{id} | Get website theme by ID
[**get_website_themes_async**](WebsiteThemesApi.md#get_website_themes_async) | **GET** /api/v2/ContentService/WebsiteThemes | Get all website themes
[**get_website_themes_count_async**](WebsiteThemesApi.md#get_website_themes_count_async) | **GET** /api/v2/ContentService/WebsiteThemes/Count | Get website themes count
[**patch_website_theme_async**](WebsiteThemesApi.md#patch_website_theme_async) | **PATCH** /api/v2/ContentService/WebsiteThemes/{id} | Patch a website theme
[**update_website_theme_async**](WebsiteThemesApi.md#update_website_theme_async) | **PUT** /api/v2/ContentService/WebsiteThemes/{id} | Update a website theme



## create_website_theme_async

> create_website_theme_async(tenant_id, api_version, x_api_version, website_theme_create_dto)
Create a new website theme

Creates a new website theme for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**website_theme_create_dto** | Option<[**WebsiteThemeCreateDto**](WebsiteThemeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_website_theme_async

> delete_website_theme_async(tenant_id, id, api_version, x_api_version)
Delete a website theme

Deletes a website theme for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_website_theme_by_id_async

> models::WebsiteThemeDto get_website_theme_by_id_async(tenant_id, id, api_version, x_api_version)
Get website theme by ID

Retrieves a specific website theme by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebsiteThemeDto**](WebsiteThemeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_website_themes_async

> models::WebsiteThemeDtoListEnvelope get_website_themes_async(tenant_id, api_version, x_api_version, website_theme_dto_collection_query_parameters)
Get all website themes

Retrieves all website themes for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**website_theme_dto_collection_query_parameters** | Option<[**WebsiteThemeDtoCollectionQueryParameters**](WebsiteThemeDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::WebsiteThemeDtoListEnvelope**](WebsiteThemeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_website_themes_count_async

> models::Int32Envelope get_website_themes_count_async(tenant_id, api_version, x_api_version, website_theme_dto_collection_query_parameters)
Get website themes count

Returns the count of website themes for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**website_theme_dto_collection_query_parameters** | Option<[**WebsiteThemeDtoCollectionQueryParameters**](WebsiteThemeDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_website_theme_async

> patch_website_theme_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a website theme

Partially updates an existing website theme for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_website_theme_async

> update_website_theme_async(tenant_id, id, api_version, x_api_version, website_theme_update_dto)
Update a website theme

Updates an existing website theme for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**website_theme_update_dto** | Option<[**WebsiteThemeUpdateDto**](WebsiteThemeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

