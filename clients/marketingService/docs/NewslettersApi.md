# \NewslettersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_newsletter_async**](NewslettersApi.md#create_newsletter_async) | **POST** /api/v2/MarketingService/Newsletters | Create a newsletter
[**delete_newsletter_async**](NewslettersApi.md#delete_newsletter_async) | **DELETE** /api/v2/MarketingService/Newsletters/{newsletterId} | Delete a newsletter
[**get_newsletter_details_async**](NewslettersApi.md#get_newsletter_details_async) | **GET** /api/v2/MarketingService/Newsletters/{newsletterId} | Get newsletter by ID
[**get_newsletter_o_data_async**](NewslettersApi.md#get_newsletter_o_data_async) | **GET** /api/v2/MarketingService/Newsletters | Get newsletters
[**get_newsletters_count_async**](NewslettersApi.md#get_newsletters_count_async) | **GET** /api/v2/MarketingService/Newsletters/Count | Get newsletters count
[**update_newsletter_async**](NewslettersApi.md#update_newsletter_async) | **PUT** /api/v2/MarketingService/Newsletters/{newsletterId} | Update a newsletter



## create_newsletter_async

> models::EmptyEnvelope create_newsletter_async(tenant_id, newsletter_create_dto, api_version, x_api_version)
Create a newsletter

Creates a new newsletter for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_create_dto** | [**NewsletterCreateDto**](NewsletterCreateDto.md) |  | [required] |
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


## delete_newsletter_async

> models::EmptyEnvelope delete_newsletter_async(tenant_id, newsletter_id, api_version, x_api_version)
Delete a newsletter

Deletes a newsletter by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_id** | **uuid::Uuid** |  | [required] |
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


## get_newsletter_details_async

> models::NewsletterDtoEnvelope get_newsletter_details_async(tenant_id, newsletter_id, api_version, x_api_version)
Get newsletter by ID

Retrieves the details of a specific newsletter by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NewsletterDtoEnvelope**](NewsletterDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_newsletter_o_data_async

> get_newsletter_o_data_async(tenant_id, api_version, x_api_version)
Get newsletters

Retrieves a collection of newsletters for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
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


## get_newsletters_count_async

> models::Int32Envelope get_newsletters_count_async(tenant_id, api_version, x_api_version)
Get newsletters count

Returns the count of newsletters for the specified tenant using OData query options.

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


## update_newsletter_async

> models::EmptyEnvelope update_newsletter_async(tenant_id, newsletter_id, newsletter_update_dto, api_version, x_api_version)
Update a newsletter

Updates an existing newsletter by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**newsletter_id** | **uuid::Uuid** |  | [required] |
**newsletter_update_dto** | [**NewsletterUpdateDto**](NewsletterUpdateDto.md) |  | [required] |
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

