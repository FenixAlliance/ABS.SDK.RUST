# \WebTemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_web_templates_async**](WebTemplatesApi.md#count_web_templates_async) | **GET** /api/v2/ContentService/WebTemplates/Count | Count web templates
[**create_web_template_async**](WebTemplatesApi.md#create_web_template_async) | **POST** /api/v2/ContentService/WebTemplates | Create a web template
[**delete_web_template_async**](WebTemplatesApi.md#delete_web_template_async) | **DELETE** /api/v2/ContentService/WebTemplates/{webTemplateId} | Delete a web template
[**get_web_template_by_id_async**](WebTemplatesApi.md#get_web_template_by_id_async) | **GET** /api/v2/ContentService/WebTemplates/{webTemplateId} | Get web template by ID
[**get_web_templates_async**](WebTemplatesApi.md#get_web_templates_async) | **GET** /api/v2/ContentService/WebTemplates | Get web templates
[**update_web_template_async**](WebTemplatesApi.md#update_web_template_async) | **PUT** /api/v2/ContentService/WebTemplates/{webTemplateId} | Update a web template



## count_web_templates_async

> models::Int32Envelope count_web_templates_async(tenant_id, api_version, x_api_version)
Count web templates

Counts all web templates for the specified tenant.

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


## create_web_template_async

> create_web_template_async(tenant_id, api_version, x_api_version, web_template_create_dto)
Create a web template

Creates a new web template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_template_create_dto** | Option<[**WebTemplateCreateDto**](WebTemplateCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_template_async

> delete_web_template_async(tenant_id, web_template_id, api_version, x_api_version)
Delete a web template

Deletes a web template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_template_id** | **uuid::Uuid** |  | [required] |
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


## get_web_template_by_id_async

> models::WebTemplateDtoEnvelope get_web_template_by_id_async(tenant_id, web_template_id, api_version, x_api_version)
Get web template by ID

Retrieves a specific web template by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_template_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebTemplateDtoEnvelope**](WebTemplateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_templates_async

> models::WebTemplateDtoListEnvelope get_web_templates_async(tenant_id, api_version, x_api_version)
Get web templates

Retrieves all web templates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebTemplateDtoListEnvelope**](WebTemplateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_web_template_async

> update_web_template_async(tenant_id, web_template_id, api_version, x_api_version, web_template_update_dto)
Update a web template

Updates an existing web template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**web_template_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_template_update_dto** | Option<[**WebTemplateUpdateDto**](WebTemplateUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

