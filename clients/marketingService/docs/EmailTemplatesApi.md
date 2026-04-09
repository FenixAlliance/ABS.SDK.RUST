# \EmailTemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_email_template_async**](EmailTemplatesApi.md#create_email_template_async) | **POST** /api/v2/MarketingService/EmailTemplates | Create an email template
[**delete_email_template_async**](EmailTemplatesApi.md#delete_email_template_async) | **DELETE** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Delete an email template
[**get_email_template_details_async**](EmailTemplatesApi.md#get_email_template_details_async) | **GET** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Get email template by ID
[**get_email_templates_count_async**](EmailTemplatesApi.md#get_email_templates_count_async) | **GET** /api/v2/MarketingService/EmailTemplates/Count | Get email templates count
[**get_email_templates_o_data_async**](EmailTemplatesApi.md#get_email_templates_o_data_async) | **GET** /api/v2/MarketingService/EmailTemplates | Get email templates
[**update_email_template_async**](EmailTemplatesApi.md#update_email_template_async) | **PUT** /api/v2/MarketingService/EmailTemplates/{emailTemplateId} | Update an email template



## create_email_template_async

> models::EmptyEnvelope create_email_template_async(tenant_id, email_template_create_dto, api_version, x_api_version)
Create an email template

Creates a new email template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_template_create_dto** | [**EmailTemplateCreateDto**](EmailTemplateCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_email_template_async

> models::EmptyEnvelope delete_email_template_async(tenant_id, email_template_id, api_version, x_api_version)
Delete an email template

Deletes an email template by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_template_id** | **uuid::Uuid** |  | [required] |
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


## get_email_template_details_async

> models::EmailTemplateDtoEnvelope get_email_template_details_async(tenant_id, email_template_id, api_version, x_api_version)
Get email template by ID

Retrieves the details of a specific email template by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_template_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailTemplateDtoEnvelope**](EmailTemplateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_email_templates_count_async

> models::Int32Envelope get_email_templates_count_async(tenant_id, api_version, x_api_version)
Get email templates count

Returns the count of email templates for the specified tenant using OData query options.

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


## get_email_templates_o_data_async

> models::EmailTemplateDtoListEnvelope get_email_templates_o_data_async(tenant_id, api_version, x_api_version)
Get email templates

Retrieves a collection of email templates for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailTemplateDtoListEnvelope**](EmailTemplateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_email_template_async

> models::EmptyEnvelope update_email_template_async(tenant_id, email_template_id, email_template_update_dto, api_version, x_api_version)
Update an email template

Updates an existing email template by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_template_id** | **uuid::Uuid** |  | [required] |
**email_template_update_dto** | [**EmailTemplateUpdateDto**](EmailTemplateUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

