# \LicensesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_license_async**](LicensesApi.md#create_license_async) | **POST** /api/v2/LicensingService/Licenses | Create a new license
[**delete_license_async**](LicensesApi.md#delete_license_async) | **DELETE** /api/v2/LicensingService/Licenses/{licenseId} | Delete a license
[**get_license_by_id_async**](LicensesApi.md#get_license_by_id_async) | **GET** /api/v2/LicensingService/Licenses/{licenseId} | Get license by ID
[**get_licenses_async**](LicensesApi.md#get_licenses_async) | **GET** /api/v2/LicensingService/Licenses | Get licenses
[**get_licenses_count_async**](LicensesApi.md#get_licenses_count_async) | **GET** /api/v2/LicensingService/Licenses/Count | Get licenses count
[**update_license_async**](LicensesApi.md#update_license_async) | **PUT** /api/v2/LicensingService/Licenses/{licenseId} | Update a license



## create_license_async

> create_license_async(tenant_id, api_version, x_api_version, license_create_dto)
Create a new license

Creates a new license instance for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_create_dto** | Option<[**LicenseCreateDto**](LicenseCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_license_async

> delete_license_async(tenant_id, license_id, api_version, x_api_version)
Delete a license

Deletes a license instance for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
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


## get_license_by_id_async

> models::LicenseDto get_license_by_id_async(tenant_id, license_id, api_version, x_api_version)
Get license by ID

Retrieves a specific license instance by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseDto**](LicenseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_licenses_async

> models::LicenseDtoListEnvelope get_licenses_async(tenant_id, api_version, x_api_version, license_dto_collection_query_parameters)
Get licenses

Retrieves the license instances owned by the specified tenant, filtered via OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_dto_collection_query_parameters** | Option<[**LicenseDtoCollectionQueryParameters**](LicenseDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::LicenseDtoListEnvelope**](LicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_licenses_count_async

> models::Int32Envelope get_licenses_count_async(tenant_id, api_version, x_api_version, license_dto_collection_query_parameters)
Get licenses count

Returns the count of license instances owned by the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_dto_collection_query_parameters** | Option<[**LicenseDtoCollectionQueryParameters**](LicenseDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_license_async

> update_license_async(tenant_id, license_id, api_version, x_api_version, license_update_dto)
Update a license

Updates an existing license instance for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**license_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_update_dto** | Option<[**LicenseUpdateDto**](LicenseUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

