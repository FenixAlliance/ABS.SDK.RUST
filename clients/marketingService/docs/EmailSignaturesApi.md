# \EmailSignaturesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_email_signature_async**](EmailSignaturesApi.md#create_email_signature_async) | **POST** /api/v2/MarketingService/EmailSignatures | Create an email signature
[**delete_email_signature_async**](EmailSignaturesApi.md#delete_email_signature_async) | **DELETE** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Delete an email signature
[**get_email_signature_details_async**](EmailSignaturesApi.md#get_email_signature_details_async) | **GET** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Get email signature by ID
[**get_email_signatures_count_async**](EmailSignaturesApi.md#get_email_signatures_count_async) | **GET** /api/v2/MarketingService/EmailSignatures/Count | Get email signatures count
[**get_email_signatures_o_data_async**](EmailSignaturesApi.md#get_email_signatures_o_data_async) | **GET** /api/v2/MarketingService/EmailSignatures | Get email signatures
[**update_email_signature_async**](EmailSignaturesApi.md#update_email_signature_async) | **PUT** /api/v2/MarketingService/EmailSignatures/{emailsignatureId} | Update an email signature



## create_email_signature_async

> models::EmptyEnvelope create_email_signature_async(tenant_id, email_signature_create_dto, api_version, x_api_version)
Create an email signature

Creates a new email signature for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_signature_create_dto** | [**EmailSignatureCreateDto**](EmailSignatureCreateDto.md) |  | [required] |
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


## delete_email_signature_async

> models::EmptyEnvelope delete_email_signature_async(tenant_id, emailsignature_id, api_version, x_api_version)
Delete an email signature

Deletes an email signature by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailsignature_id** | **uuid::Uuid** |  | [required] |
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


## get_email_signature_details_async

> models::EmailSignatureDtoEnvelope get_email_signature_details_async(tenant_id, emailsignature_id, api_version, x_api_version)
Get email signature by ID

Retrieves the details of a specific email signature by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailsignature_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailSignatureDtoEnvelope**](EmailSignatureDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_email_signatures_count_async

> models::Int32Envelope get_email_signatures_count_async(tenant_id, api_version, x_api_version)
Get email signatures count

Returns the count of email signatures for the specified tenant using OData query options.

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


## get_email_signatures_o_data_async

> models::EmailSignatureDtoListEnvelope get_email_signatures_o_data_async(tenant_id, api_version, x_api_version)
Get email signatures

Retrieves a collection of email signatures for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmailSignatureDtoListEnvelope**](EmailSignatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_email_signature_async

> models::EmptyEnvelope update_email_signature_async(tenant_id, emailsignature_id, email_signature_update_dto, api_version, x_api_version)
Update an email signature

Updates an existing email signature by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**emailsignature_id** | **uuid::Uuid** |  | [required] |
**email_signature_update_dto** | [**EmailSignatureUpdateDto**](EmailSignatureUpdateDto.md) |  | [required] |
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

