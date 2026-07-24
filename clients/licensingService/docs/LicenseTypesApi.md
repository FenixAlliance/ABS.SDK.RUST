# \LicenseTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_license_type_async**](LicenseTypesApi.md#create_license_type_async) | **POST** /api/v2/LicensingService/LicenseTypes | Create a new license type
[**delete_license_type_async**](LicenseTypesApi.md#delete_license_type_async) | **DELETE** /api/v2/LicensingService/LicenseTypes/{id} | Delete a license type
[**get_license_type_by_id_async**](LicenseTypesApi.md#get_license_type_by_id_async) | **GET** /api/v2/LicensingService/LicenseTypes/{id} | Get license type by ID
[**get_license_types_async**](LicenseTypesApi.md#get_license_types_async) | **GET** /api/v2/LicensingService/LicenseTypes | Get all license types
[**get_license_types_count_async**](LicenseTypesApi.md#get_license_types_count_async) | **GET** /api/v2/LicensingService/LicenseTypes/Count | Get license types count
[**patch_license_type_async**](LicenseTypesApi.md#patch_license_type_async) | **PATCH** /api/v2/LicensingService/LicenseTypes/{id} | Patch a license type
[**update_license_type_async**](LicenseTypesApi.md#update_license_type_async) | **PUT** /api/v2/LicensingService/LicenseTypes/{id} | Update a license type



## create_license_type_async

> create_license_type_async(tenant_id, api_version, x_api_version, license_type_create_dto)
Create a new license type

Creates a new license type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_type_create_dto** | Option<[**LicenseTypeCreateDto**](LicenseTypeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_license_type_async

> delete_license_type_async(tenant_id, id, api_version, x_api_version)
Delete a license type

Deletes a license type for the specified tenant.

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


## get_license_type_by_id_async

> models::LicenseTypeDto get_license_type_by_id_async(tenant_id, id, api_version, x_api_version)
Get license type by ID

Retrieves a specific license type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseTypeDto**](LicenseTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_types_async

> models::LicenseTypeDtoListEnvelope get_license_types_async(tenant_id, api_version, x_api_version)
Get all license types

Retrieves all license types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseTypeDtoListEnvelope**](LicenseTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_types_count_async

> models::Int32Envelope get_license_types_count_async(tenant_id, api_version, x_api_version)
Get license types count

Returns the count of license types for the specified tenant.

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


## patch_license_type_async

> models::EmptyEnvelope patch_license_type_async(tenant_id, id, api_version, x_api_version, operation)
Patch a license type

Patch a license type for the specified tenant.

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


## update_license_type_async

> update_license_type_async(tenant_id, id, api_version, x_api_version, license_type_update_dto)
Update a license type

Updates an existing license type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_type_update_dto** | Option<[**LicenseTypeUpdateDto**](LicenseTypeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

