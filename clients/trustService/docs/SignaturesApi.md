# \SignaturesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_signature_by_id_async**](SignaturesApi.md#get_signature_by_id_async) | **GET** /api/v2/TrustService/Signatures/{id} | Get signature by ID
[**get_signatures_async**](SignaturesApi.md#get_signatures_async) | **GET** /api/v2/TrustService/Signatures | Get all signatures
[**get_signatures_count_async**](SignaturesApi.md#get_signatures_count_async) | **GET** /api/v2/TrustService/Signatures/Count | Get signatures count



## get_signature_by_id_async

> models::SignatureDto get_signature_by_id_async(tenant_id, id, api_version, x_api_version)
Get signature by ID

Retrieves a specific signature by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SignatureDto**](SignatureDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signatures_async

> models::SignatureDtoListEnvelope get_signatures_async(tenant_id, api_version, x_api_version, signature_dto_collection_query_parameters)
Get all signatures

Retrieves all signatures for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signature_dto_collection_query_parameters** | Option<[**SignatureDtoCollectionQueryParameters**](SignatureDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::SignatureDtoListEnvelope**](SignatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signatures_count_async

> models::Int32Envelope get_signatures_count_async(tenant_id, api_version, x_api_version, signature_dto_collection_query_parameters)
Get signatures count

Returns the count of signatures for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signature_dto_collection_query_parameters** | Option<[**SignatureDtoCollectionQueryParameters**](SignatureDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

