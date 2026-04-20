# \PaymentTermsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_term_async**](PaymentTermsApi.md#create_payment_term_async) | **POST** /api/v2/PaymentsService/PaymentTerms | Creates a new payment term
[**delete_payment_term_async**](PaymentTermsApi.md#delete_payment_term_async) | **DELETE** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Deletes a payment term
[**get_payment_term_details_async**](PaymentTermsApi.md#get_payment_term_details_async) | **GET** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Gets a payment term by ID
[**get_payment_terms_async**](PaymentTermsApi.md#get_payment_terms_async) | **GET** /api/v2/PaymentsService/PaymentTerms | Retrieves all payment terms
[**get_payment_terms_count_async**](PaymentTermsApi.md#get_payment_terms_count_async) | **GET** /api/v2/PaymentsService/PaymentTerms/Count | Counts payment terms
[**update_payment_term_async**](PaymentTermsApi.md#update_payment_term_async) | **PUT** /api/v2/PaymentsService/PaymentTerms/{paymentTermId} | Updates a payment term



## create_payment_term_async

> models::EmptyEnvelope create_payment_term_async(tenant_id, api_version, x_api_version, payment_term_create_dto)
Creates a new payment term

Creates a new payment term for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_term_create_dto** | Option<[**PaymentTermCreateDto**](PaymentTermCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payment_term_async

> models::EmptyEnvelope delete_payment_term_async(tenant_id, payment_term_id, api_version, x_api_version)
Deletes a payment term

Deletes the specified payment term.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_term_id** | **uuid::Uuid** |  | [required] |
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


## get_payment_term_details_async

> models::PaymentTermDtoEnvelope get_payment_term_details_async(tenant_id, payment_term_id, api_version, x_api_version)
Gets a payment term by ID

Retrieves the details of a payment term using its unique ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_term_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentTermDtoEnvelope**](PaymentTermDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_terms_async

> models::PaymentTermDtoIReadOnlyListEnvelope get_payment_terms_async(tenant_id, api_version, x_api_version)
Retrieves all payment terms

Gets all payment terms for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentTermDtoIReadOnlyListEnvelope**](PaymentTermDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_terms_count_async

> models::Int32Envelope get_payment_terms_count_async(tenant_id, api_version, x_api_version)
Counts payment terms

Gets the count of payment terms for the current tenant.

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


## update_payment_term_async

> models::EmptyEnvelope update_payment_term_async(tenant_id, payment_term_id, api_version, x_api_version, payment_term_update_dto)
Updates a payment term

Updates the specified payment term.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_term_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_term_update_dto** | Option<[**PaymentTermUpdateDto**](PaymentTermUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

