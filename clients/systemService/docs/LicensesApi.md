# \LicensesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_licensing_licenses_generate_post**](LicensesApi.md#api_licensing_licenses_generate_post) | **POST** /api/Licensing/Licenses/Generate | 
[**api_licensing_licenses_validate_attributes_get**](LicensesApi.md#api_licensing_licenses_validate_attributes_get) | **GET** /api/Licensing/Licenses/Validate/Attributes | 
[**api_licensing_licenses_validate_errors_get**](LicensesApi.md#api_licensing_licenses_validate_errors_get) | **GET** /api/Licensing/Licenses/Validate/Errors | 
[**api_licensing_licenses_validate_get**](LicensesApi.md#api_licensing_licenses_validate_get) | **GET** /api/Licensing/Licenses/Validate | 



## api_licensing_licenses_generate_post

> models::StringEnvelope api_licensing_licenses_generate_post(tenant_id, api_version, x_api_version, license_key_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_key_request** | Option<[**LicenseKeyRequest**](LicenseKeyRequest.md)> |  |  |

### Return type

[**models::StringEnvelope**](StringEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_licensing_licenses_validate_attributes_get

> models::LicenseAttributesListEnvelope api_licensing_licenses_validate_attributes_get(tenant_id, api_version, x_api_version, license_key)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_key** | Option<[**LicenseKey**](LicenseKey.md)> |  |  |

### Return type

[**models::LicenseAttributesListEnvelope**](LicenseAttributesListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_licensing_licenses_validate_errors_get

> models::LicenseValidationErrorListEnvelope api_licensing_licenses_validate_errors_get(tenant_id, api_version, x_api_version, license_key)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_key** | Option<[**LicenseKey**](LicenseKey.md)> |  |  |

### Return type

[**models::LicenseValidationErrorListEnvelope**](LicenseValidationErrorListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## api_licensing_licenses_validate_get

> models::BooleanEnvelope api_licensing_licenses_validate_get(tenant_id, api_version, x_api_version, license_key)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_key** | Option<[**LicenseKey**](LicenseKey.md)> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

