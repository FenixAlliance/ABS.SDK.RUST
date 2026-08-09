# \PaymentProviderRegistrationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_async**](PaymentProviderRegistrationsApi.md#create_async) | **POST** /api/v2/PaymentsService/PaymentProviderRegistrations | Provisions a provider webhook registration
[**get_async**](PaymentProviderRegistrationsApi.md#get_async) | **GET** /api/v2/PaymentsService/PaymentProviderRegistrations | Lists the tenant's provider registrations
[**get_count_async**](PaymentProviderRegistrationsApi.md#get_count_async) | **GET** /api/v2/PaymentsService/PaymentProviderRegistrations/Count | Counts the tenant's provider registrations
[**rotate_key_async**](PaymentProviderRegistrationsApi.md#rotate_key_async) | **POST** /api/v2/PaymentsService/PaymentProviderRegistrations/{registrationId}/RotateKey | Rotates a registration's webhook key



## create_async

> models::ProviderWebhookRegistrationCreatedDtoEnvelope create_async(tenant_id, create_provider_webhook_registration_request)
Provisions a provider webhook registration

Stores the BYO signing secret in the tenant options store, creates + activates the registration, and reveals the one-time plaintext webhook key plus its fully-composed inbound URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**create_provider_webhook_registration_request** | Option<[**CreateProviderWebhookRegistrationRequest**](CreateProviderWebhookRegistrationRequest.md)> |  |  |

### Return type

[**models::ProviderWebhookRegistrationCreatedDtoEnvelope**](ProviderWebhookRegistrationCreatedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_async

> models::PaymentProviderRegistrationDtoListEnvelope get_async(tenant_id, payment_provider_registration_dto_collection_query_parameters)
Lists the tenant's provider registrations

Gets all provider registrations for the current tenant with OData support (no secret is ever returned).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_provider_registration_dto_collection_query_parameters** | Option<[**PaymentProviderRegistrationDtoCollectionQueryParameters**](PaymentProviderRegistrationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::PaymentProviderRegistrationDtoListEnvelope**](PaymentProviderRegistrationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_count_async

> models::Int32Envelope get_count_async(tenant_id, payment_provider_registration_dto_collection_query_parameters)
Counts the tenant's provider registrations

Gets the count of provider registrations for the current tenant (OData sibling of the list).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_provider_registration_dto_collection_query_parameters** | Option<[**PaymentProviderRegistrationDtoCollectionQueryParameters**](PaymentProviderRegistrationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## rotate_key_async

> models::ProviderWebhookRegistrationCreatedDtoEnvelope rotate_key_async(tenant_id, registration_id)
Rotates a registration's webhook key

Mints a fresh webhook key (invalidating the previous one) and reveals it once, plus its composed URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**registration_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ProviderWebhookRegistrationCreatedDtoEnvelope**](ProviderWebhookRegistrationCreatedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

