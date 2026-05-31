# \WebContentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_web_contents_async**](WebContentsApi.md#count_web_contents_async) | **GET** /api/v2/ContentService/WebContents/Count | Count web contents
[**create_web_content_async**](WebContentsApi.md#create_web_content_async) | **POST** /api/v2/ContentService/WebContents | Create a web content
[**delete_web_content_async**](WebContentsApi.md#delete_web_content_async) | **DELETE** /api/v2/ContentService/WebContents/{webContentId} | Delete a web content
[**get_web_content_by_id_async**](WebContentsApi.md#get_web_content_by_id_async) | **GET** /api/v2/ContentService/WebContents/{webContentId} | Get web content by ID
[**get_web_contents_async**](WebContentsApi.md#get_web_contents_async) | **GET** /api/v2/ContentService/WebContents | Get web contents
[**update_web_content_async**](WebContentsApi.md#update_web_content_async) | **PUT** /api/v2/ContentService/WebContents/{webContentId} | Update a web content



## count_web_contents_async

> models::Int32Envelope count_web_contents_async(tenant_id, api_version, x_api_version)
Count web contents

Counts all web contents for the specified tenant.

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


## create_web_content_async

> models::EmptyEnvelope create_web_content_async(tenant_id, api_version, x_api_version, web_content_create_dto)
Create a web content

Creates a new web content for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_content_create_dto** | Option<[**WebContentCreateDto**](WebContentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_content_async

> models::EmptyEnvelope delete_web_content_async(tenant_id, web_content_id, api_version, x_api_version)
Delete a web content

Deletes a web content for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_content_id** | **uuid::Uuid** |  | [required] |
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


## get_web_content_by_id_async

> models::WebContentDtoEnvelope get_web_content_by_id_async(tenant_id, web_content_id, api_version, x_api_version)
Get web content by ID

Retrieves a specific web content by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_content_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebContentDtoEnvelope**](WebContentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_contents_async

> models::WebContentDtoListEnvelope get_web_contents_async(tenant_id, api_version, x_api_version)
Get web contents

Retrieves all web contents for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebContentDtoListEnvelope**](WebContentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_web_content_async

> models::EmptyEnvelope update_web_content_async(tenant_id, web_content_id, api_version, x_api_version, web_content_update_dto)
Update a web content

Updates an existing web content for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_content_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_content_update_dto** | Option<[**WebContentUpdateDto**](WebContentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

