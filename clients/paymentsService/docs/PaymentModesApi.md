# \PaymentModesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_mode_async**](PaymentModesApi.md#create_payment_mode_async) | **POST** /api/v2/PaymentsService/PaymentModes | Creates a new payment mode
[**delete_payment_mode_async**](PaymentModesApi.md#delete_payment_mode_async) | **DELETE** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Deletes a payment mode
[**get_payment_mode_details_async**](PaymentModesApi.md#get_payment_mode_details_async) | **GET** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Gets a payment mode by ID
[**get_payment_modes_async**](PaymentModesApi.md#get_payment_modes_async) | **GET** /api/v2/PaymentsService/PaymentModes | Retrieves all payment modes
[**get_payment_modes_count_async**](PaymentModesApi.md#get_payment_modes_count_async) | **GET** /api/v2/PaymentsService/PaymentModes/Count | Counts payment modes
[**update_payment_mode_async**](PaymentModesApi.md#update_payment_mode_async) | **PUT** /api/v2/PaymentsService/PaymentModes/{paymentModeId} | Updates a payment mode



## create_payment_mode_async

> models::EmptyEnvelope create_payment_mode_async(tenant_id, api_version, x_api_version, payment_mode_create_dto)
Creates a new payment mode

Creates a new payment mode for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_mode_create_dto** | Option<[**PaymentModeCreateDto**](PaymentModeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payment_mode_async

> models::EmptyEnvelope delete_payment_mode_async(tenant_id, payment_mode_id, api_version, x_api_version)
Deletes a payment mode

Deletes the specified payment mode.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_mode_id** | **uuid::Uuid** |  | [required] |
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


## get_payment_mode_details_async

> models::PaymentModeDtoEnvelope get_payment_mode_details_async(tenant_id, payment_mode_id, api_version, x_api_version)
Gets a payment mode by ID

Retrieves the details of a payment mode using its unique ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_mode_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentModeDtoEnvelope**](PaymentModeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_modes_async

> models::PaymentModeDtoIReadOnlyListEnvelope get_payment_modes_async(tenant_id, api_version, x_api_version)
Retrieves all payment modes

Gets all payment modes for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentModeDtoIReadOnlyListEnvelope**](PaymentModeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_modes_count_async

> models::Int32Envelope get_payment_modes_count_async(tenant_id, api_version, x_api_version)
Counts payment modes

Gets the count of payment modes for the current tenant.

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


## update_payment_mode_async

> models::EmptyEnvelope update_payment_mode_async(tenant_id, payment_mode_id, api_version, x_api_version, payment_mode_update_dto)
Updates a payment mode

Updates the specified payment mode.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**payment_mode_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_mode_update_dto** | Option<[**PaymentModeUpdateDto**](PaymentModeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

