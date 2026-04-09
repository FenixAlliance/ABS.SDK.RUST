# \PaymentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_async**](PaymentsApi.md#create_payment_async) | **POST** /api/v2/PaymentsService/Payments | Creates a new payment
[**delete_payment_async**](PaymentsApi.md#delete_payment_async) | **DELETE** /api/v2/PaymentsService/Payments/{paymentId} | Deletes a payment
[**get_payment_async**](PaymentsApi.md#get_payment_async) | **GET** /api/v2/PaymentsService/Payments/{paymentId}/Details | Gets a payment by ID (deprecated)
[**get_payment_async_v2**](PaymentsApi.md#get_payment_async_v2) | **GET** /api/v2/PaymentsService/Payments/{paymentId} | Gets a payment by ID
[**get_payments_async**](PaymentsApi.md#get_payments_async) | **GET** /api/v2/PaymentsService/Payments | Retrieves all payments
[**update_payment_async**](PaymentsApi.md#update_payment_async) | **PUT** /api/v2/PaymentsService/Payments/{paymentId} | Updates a payment



## create_payment_async

> models::EmptyEnvelope create_payment_async(tenant_id, payment_create_dto)
Creates a new payment

Creates a new payment for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_create_dto** | Option<[**PaymentCreateDto**](PaymentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payment_async

> models::EmptyEnvelope delete_payment_async(tenant_id, payment_id)
Deletes a payment

Deletes the specified payment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_async

> models::PaymentDtoListEnvelope get_payment_async(payment_id)
Gets a payment by ID (deprecated)

Retrieves a payment using the deprecated /Details route. Use GET {paymentId} instead.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_async_v2

> models::PaymentDtoListEnvelope get_payment_async_v2(payment_id)
Gets a payment by ID

Retrieves the details of a payment using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**payment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payments_async

> models::PaymentDtoListEnvelope get_payments_async(tenant_id)
Retrieves all payments

Gets all payments for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_payment_async

> models::EmptyEnvelope update_payment_async(tenant_id, payment_id, payment_update_dto)
Updates a payment

Updates the specified payment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_id** | **uuid::Uuid** |  | [required] |
**payment_update_dto** | Option<[**PaymentUpdateDto**](PaymentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

