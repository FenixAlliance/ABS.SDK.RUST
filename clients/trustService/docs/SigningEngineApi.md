# \SigningEngineApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_providers_async**](SigningEngineApi.md#get_providers_async) | **GET** /api/v2/TrustService/SigningEngine/Providers | List signing providers
[**get_providers_count_async**](SigningEngineApi.md#get_providers_count_async) | **GET** /api/v2/TrustService/SigningEngine/Providers/Count | Count signing providers
[**preview_async**](SigningEngineApi.md#preview_async) | **POST** /api/v2/TrustService/SigningEngine/Preview | Preview signing readiness



## get_providers_async

> models::TrustSigningProviderDescriptorDtoListEnvelope get_providers_async(tenant_id, api_version, x_api_version, trust_signing_provider_descriptor_dto_collection_query_parameters)
List signing providers

Returns the registered alpha signing providers (Noop / Manual / External). OData-queryable.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**trust_signing_provider_descriptor_dto_collection_query_parameters** | Option<[**TrustSigningProviderDescriptorDtoCollectionQueryParameters**](TrustSigningProviderDescriptorDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::TrustSigningProviderDescriptorDtoListEnvelope**](TrustSigningProviderDescriptorDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_providers_count_async

> models::Int32Envelope get_providers_count_async(tenant_id, api_version, x_api_version, trust_signing_provider_descriptor_dto_collection_query_parameters)
Count signing providers

Returns the count of registered alpha signing providers. OData-queryable.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**trust_signing_provider_descriptor_dto_collection_query_parameters** | Option<[**TrustSigningProviderDescriptorDtoCollectionQueryParameters**](TrustSigningProviderDescriptorDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## preview_async

> models::TrustSigningReadinessDtoEnvelope preview_async(tenant_id, api_version, x_api_version, trust_signing_request_dto)
Preview signing readiness

Side-effect-free: validates a signing request and reports whether it can proceed and with what policy.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**trust_signing_request_dto** | Option<[**TrustSigningRequestDto**](TrustSigningRequestDto.md)> |  |  |

### Return type

[**models::TrustSigningReadinessDtoEnvelope**](TrustSigningReadinessDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

