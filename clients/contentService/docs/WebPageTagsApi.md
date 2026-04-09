# \WebPageTagsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_web_page_tag_async**](WebPageTagsApi.md#create_web_page_tag_async) | **POST** /api/v2/ContentService/WebPageTags | Create a web page tag
[**delete_web_page_tag_async**](WebPageTagsApi.md#delete_web_page_tag_async) | **DELETE** /api/v2/ContentService/WebPageTags/{webPageTagId} | Delete a web page tag
[**get_web_page_tag_by_id_async**](WebPageTagsApi.md#get_web_page_tag_by_id_async) | **GET** /api/v2/ContentService/WebPageTags/{webPageTagId} | Get web page tag by ID
[**get_web_page_tags_async**](WebPageTagsApi.md#get_web_page_tags_async) | **GET** /api/v2/ContentService/WebPageTags | Get web page tags
[**update_web_page_tag_async**](WebPageTagsApi.md#update_web_page_tag_async) | **PUT** /api/v2/ContentService/WebPageTags/{webPageTagId} | Update a web page tag



## create_web_page_tag_async

> models::EmptyEnvelope create_web_page_tag_async(tenant_id, api_version, x_api_version, web_page_tag_create_dto)
Create a web page tag

Creates a new web page tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_tag_create_dto** | Option<[**WebPageTagCreateDto**](WebPageTagCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_page_tag_async

> models::EmptyEnvelope delete_web_page_tag_async(tenant_id, web_page_tag_id, api_version, x_api_version)
Delete a web page tag

Deletes a web page tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_tag_id** | **uuid::Uuid** |  | [required] |
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


## get_web_page_tag_by_id_async

> models::WebPageTagDtoEnvelope get_web_page_tag_by_id_async(tenant_id, web_page_tag_id, api_version, x_api_version)
Get web page tag by ID

Retrieves a specific web page tag by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPageTagDtoEnvelope**](WebPageTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_page_tags_async

> models::WebPageTagDtoListEnvelope get_web_page_tags_async(tenant_id, api_version, x_api_version)
Get web page tags

Retrieves all web page tags for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## update_web_page_tag_async

> models::EmptyEnvelope update_web_page_tag_async(tenant_id, web_page_tag_id, api_version, x_api_version, web_page_tag_update_dto)
Update a web page tag

Updates an existing web page tag for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_page_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_page_tag_update_dto** | Option<[**WebPageTagUpdateDto**](WebPageTagUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

