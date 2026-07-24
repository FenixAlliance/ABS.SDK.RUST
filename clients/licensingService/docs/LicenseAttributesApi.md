# \LicenseAttributesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_license_attribute_async**](LicenseAttributesApi.md#create_license_attribute_async) | **POST** /api/v2/LicensingService/LicenseAttributes | Create a new license attribute
[**delete_license_attribute_async**](LicenseAttributesApi.md#delete_license_attribute_async) | **DELETE** /api/v2/LicensingService/LicenseAttributes/{id} | Delete a license attribute
[**get_license_attribute_by_id_async**](LicenseAttributesApi.md#get_license_attribute_by_id_async) | **GET** /api/v2/LicensingService/LicenseAttributes/{id} | Get license attribute by ID
[**get_license_attributes_async**](LicenseAttributesApi.md#get_license_attributes_async) | **GET** /api/v2/LicensingService/LicenseAttributes | Get all license attributes
[**get_license_attributes_count_async**](LicenseAttributesApi.md#get_license_attributes_count_async) | **GET** /api/v2/LicensingService/LicenseAttributes/Count | Get license attributes count
[**patch_license_attribute_async**](LicenseAttributesApi.md#patch_license_attribute_async) | **PATCH** /api/v2/LicensingService/LicenseAttributes/{id} | Patch a license attribute
[**update_license_attribute_async**](LicenseAttributesApi.md#update_license_attribute_async) | **PUT** /api/v2/LicensingService/LicenseAttributes/{id} | Update a license attribute



## create_license_attribute_async

> create_license_attribute_async(tenant_id, api_version, x_api_version, license_attribute_create_dto)
Create a new license attribute

Creates a new license attribute for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_attribute_create_dto** | Option<[**LicenseAttributeCreateDto**](LicenseAttributeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_license_attribute_async

> delete_license_attribute_async(tenant_id, id, api_version, x_api_version)
Delete a license attribute

Deletes a license attribute for the specified tenant.

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


## get_license_attribute_by_id_async

> models::LicenseAttributeDto get_license_attribute_by_id_async(tenant_id, id, api_version, x_api_version)
Get license attribute by ID

Retrieves a specific license attribute by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseAttributeDto**](LicenseAttributeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_attributes_async

> models::LicenseAttributeDtoListEnvelope get_license_attributes_async(tenant_id, api_version, x_api_version)
Get all license attributes

Retrieves all license attributes for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseAttributeDtoListEnvelope**](LicenseAttributeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_attributes_count_async

> models::Int32Envelope get_license_attributes_count_async(tenant_id, api_version, x_api_version)
Get license attributes count

Returns the count of license attributes for the specified tenant.

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


## patch_license_attribute_async

> models::EmptyEnvelope patch_license_attribute_async(tenant_id, id, api_version, x_api_version, operation)
Patch a license attribute

Patch a license attribute for the specified tenant.

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


## update_license_attribute_async

> update_license_attribute_async(tenant_id, id, api_version, x_api_version, license_attribute_update_dto)
Update a license attribute

Updates an existing license attribute for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_attribute_update_dto** | Option<[**LicenseAttributeUpdateDto**](LicenseAttributeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

