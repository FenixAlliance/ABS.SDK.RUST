# \SigningCertificatesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signing_certificate_async**](SigningCertificatesApi.md#create_signing_certificate_async) | **POST** /api/v2/TrustService/SigningCertificates | Create a new signing certificate
[**delete_signing_certificate_async**](SigningCertificatesApi.md#delete_signing_certificate_async) | **DELETE** /api/v2/TrustService/SigningCertificates/{id} | Delete a signing certificate
[**get_signing_certificate_by_id_async**](SigningCertificatesApi.md#get_signing_certificate_by_id_async) | **GET** /api/v2/TrustService/SigningCertificates/{id} | Get signing certificate by ID
[**get_signing_certificates_async**](SigningCertificatesApi.md#get_signing_certificates_async) | **GET** /api/v2/TrustService/SigningCertificates | Get all signing certificates
[**get_signing_certificates_count_async**](SigningCertificatesApi.md#get_signing_certificates_count_async) | **GET** /api/v2/TrustService/SigningCertificates/Count | Get signing certificates count
[**import_signing_certificate_async**](SigningCertificatesApi.md#import_signing_certificate_async) | **POST** /api/v2/TrustService/SigningCertificates/Import | Import a PFX/P12 signing certificate into custody
[**patch_signing_certificate_async**](SigningCertificatesApi.md#patch_signing_certificate_async) | **PATCH** /api/v2/TrustService/SigningCertificates/{id} | Patch a signing certificate
[**update_signing_certificate_async**](SigningCertificatesApi.md#update_signing_certificate_async) | **PUT** /api/v2/TrustService/SigningCertificates/{id} | Update a signing certificate



## create_signing_certificate_async

> create_signing_certificate_async(tenant_id, api_version, x_api_version, signing_certificate_create_dto)
Create a new signing certificate

Creates a new signing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_certificate_create_dto** | Option<[**SigningCertificateCreateDto**](SigningCertificateCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_signing_certificate_async

> delete_signing_certificate_async(tenant_id, id, api_version, x_api_version)
Delete a signing certificate

Deletes a signing certificate for the specified tenant.

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


## get_signing_certificate_by_id_async

> models::SigningCertificateDto get_signing_certificate_by_id_async(tenant_id, id, api_version, x_api_version)
Get signing certificate by ID

Retrieves a specific signing certificate by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningCertificateDto**](SigningCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_certificates_async

> models::SigningCertificateDtoListEnvelope get_signing_certificates_async(tenant_id, api_version, x_api_version)
Get all signing certificates

Retrieves all signing certificates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningCertificateDtoListEnvelope**](SigningCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_certificates_count_async

> models::Int32Envelope get_signing_certificates_count_async(tenant_id, api_version, x_api_version)
Get signing certificates count

Returns the count of signing certificates for the specified tenant.

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


## import_signing_certificate_async

> import_signing_certificate_async(tenant_id, api_version, x_api_version, id, file, password, title, contact_id)
Import a PFX/P12 signing certificate into custody

Parses the uploaded PFX/P12, imports the private material into the configured signing custody, and creates the certificate metadata record. The PFX and password are used only for the request — never returned or stored.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**id** | Option<**uuid::Uuid**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |
**password** | Option<**String**> |  |  |
**title** | Option<**String**> |  |  |
**contact_id** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_signing_certificate_async

> models::EmptyEnvelope patch_signing_certificate_async(tenant_id, id, api_version, x_api_version, operation)
Patch a signing certificate

Patch a signing certificate

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


## update_signing_certificate_async

> update_signing_certificate_async(tenant_id, id, api_version, x_api_version, signing_certificate_update_dto)
Update a signing certificate

Updates an existing signing certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_certificate_update_dto** | Option<[**SigningCertificateUpdateDto**](SigningCertificateUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

