# \SecurityCertificatesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_security_certificates_async**](SecurityCertificatesApi.md#get_security_certificates_async) | **GET** /api/v2/SecurityService/SecurityCertificates | Get security certificates
[**get_security_certificates_count_async**](SecurityCertificatesApi.md#get_security_certificates_count_async) | **GET** /api/v2/SecurityService/SecurityCertificates/Count | Get security certificates count



## get_security_certificates_async

> models::SecurityCertificateDtoListEnvelope get_security_certificates_async(tenant_id, api_version, x_api_version, security_certificate_dto_collection_query_parameters)
Get security certificates

Retrieves security certificates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**security_certificate_dto_collection_query_parameters** | Option<[**SecurityCertificateDtoCollectionQueryParameters**](SecurityCertificateDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::SecurityCertificateDtoListEnvelope**](SecurityCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_security_certificates_count_async

> models::Int32Envelope get_security_certificates_count_async(tenant_id, api_version, x_api_version, security_certificate_dto_collection_query_parameters)
Get security certificates count

Retrieves the count of security certificates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**security_certificate_dto_collection_query_parameters** | Option<[**SecurityCertificateDtoCollectionQueryParameters**](SecurityCertificateDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

