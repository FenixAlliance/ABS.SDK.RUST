# \LicensingCertificatesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_licensing_certificate_async**](LicensingCertificatesApi.md#create_licensing_certificate_async) | **POST** /api/v2/LicensingService/LicensingCertificates | Create a new licensing certificate
[**delete_licensing_certificate_async**](LicensingCertificatesApi.md#delete_licensing_certificate_async) | **DELETE** /api/v2/LicensingService/LicensingCertificates/{id} | Delete a licensing certificate
[**get_licensing_certificate_by_id_async**](LicensingCertificatesApi.md#get_licensing_certificate_by_id_async) | **GET** /api/v2/LicensingService/LicensingCertificates/{id} | Get licensing certificate by ID
[**get_licensing_certificates_async**](LicensingCertificatesApi.md#get_licensing_certificates_async) | **GET** /api/v2/LicensingService/LicensingCertificates | Get all licensing certificates
[**get_licensing_certificates_count_async**](LicensingCertificatesApi.md#get_licensing_certificates_count_async) | **GET** /api/v2/LicensingService/LicensingCertificates/Count | Get licensing certificates count
[**patch_licensing_certificate_async**](LicensingCertificatesApi.md#patch_licensing_certificate_async) | **PATCH** /api/v2/LicensingService/LicensingCertificates/{id} | Patch a licensing certificate
[**update_licensing_certificate_async**](LicensingCertificatesApi.md#update_licensing_certificate_async) | **PUT** /api/v2/LicensingService/LicensingCertificates/{id} | Update a licensing certificate



## create_licensing_certificate_async

> create_licensing_certificate_async(tenant_id, api_version, x_api_version, licensing_certificate_create_dto)
Create a new licensing certificate

Creates a new licensing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**licensing_certificate_create_dto** | Option<[**LicensingCertificateCreateDto**](LicensingCertificateCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_licensing_certificate_async

> delete_licensing_certificate_async(tenant_id, id, api_version, x_api_version)
Delete a licensing certificate

Deletes a licensing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_licensing_certificate_by_id_async

> models::LicensingCertificateDto get_licensing_certificate_by_id_async(tenant_id, id, api_version, x_api_version)
Get licensing certificate by ID

Retrieves a specific licensing certificate by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicensingCertificateDto**](LicensingCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_licensing_certificates_async

> models::LicensingCertificateDtoListEnvelope get_licensing_certificates_async(tenant_id, api_version, x_api_version)
Get all licensing certificates

Retrieves all licensing certificates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicensingCertificateDtoListEnvelope**](LicensingCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_licensing_certificates_count_async

> models::Int32Envelope get_licensing_certificates_count_async(tenant_id, api_version, x_api_version)
Get licensing certificates count

Returns the count of licensing certificates for the specified tenant.

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


## patch_licensing_certificate_async

> models::EmptyEnvelope patch_licensing_certificate_async(tenant_id, id, api_version, x_api_version, operation)
Patch a licensing certificate

Patch a licensing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_licensing_certificate_async

> update_licensing_certificate_async(tenant_id, id, api_version, x_api_version, licensing_certificate_update_dto)
Update a licensing certificate

Updates an existing licensing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**licensing_certificate_update_dto** | Option<[**LicensingCertificateUpdateDto**](LicensingCertificateUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

