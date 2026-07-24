# \LicenseFeaturesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_license_feature_async**](LicenseFeaturesApi.md#create_license_feature_async) | **POST** /api/v2/LicensingService/LicenseFeatures | Create a new license feature
[**delete_license_feature_async**](LicenseFeaturesApi.md#delete_license_feature_async) | **DELETE** /api/v2/LicensingService/LicenseFeatures/{id} | Delete a license feature
[**get_license_feature_by_id_async**](LicenseFeaturesApi.md#get_license_feature_by_id_async) | **GET** /api/v2/LicensingService/LicenseFeatures/{id} | Get license feature by ID
[**get_license_features_async**](LicenseFeaturesApi.md#get_license_features_async) | **GET** /api/v2/LicensingService/LicenseFeatures | Get all license features
[**get_license_features_count_async**](LicenseFeaturesApi.md#get_license_features_count_async) | **GET** /api/v2/LicensingService/LicenseFeatures/Count | Get license features count
[**patch_license_feature_async**](LicenseFeaturesApi.md#patch_license_feature_async) | **PATCH** /api/v2/LicensingService/LicenseFeatures/{id} | Patch a license feature
[**update_license_feature_async**](LicenseFeaturesApi.md#update_license_feature_async) | **PUT** /api/v2/LicensingService/LicenseFeatures/{id} | Update a license feature



## create_license_feature_async

> create_license_feature_async(tenant_id, api_version, x_api_version, license_feature_create_dto)
Create a new license feature

Creates a new license feature for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_feature_create_dto** | Option<[**LicenseFeatureCreateDto**](LicenseFeatureCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_license_feature_async

> delete_license_feature_async(tenant_id, id, api_version, x_api_version)
Delete a license feature

Deletes a license feature for the specified tenant.

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


## get_license_feature_by_id_async

> models::LicenseFeatureDto get_license_feature_by_id_async(tenant_id, id, api_version, x_api_version)
Get license feature by ID

Retrieves a specific license feature by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseFeatureDto**](LicenseFeatureDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_features_async

> models::LicenseFeatureDtoListEnvelope get_license_features_async(tenant_id, api_version, x_api_version)
Get all license features

Retrieves all license features for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LicenseFeatureDtoListEnvelope**](LicenseFeatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_license_features_count_async

> models::Int32Envelope get_license_features_count_async(tenant_id, api_version, x_api_version)
Get license features count

Returns the count of license features for the specified tenant.

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


## patch_license_feature_async

> models::EmptyEnvelope patch_license_feature_async(tenant_id, id, api_version, x_api_version, operation)
Patch a license feature

Patch a license feature for the specified tenant.

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


## update_license_feature_async

> update_license_feature_async(tenant_id, id, api_version, x_api_version, license_feature_update_dto)
Update a license feature

Updates an existing license feature for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**license_feature_update_dto** | Option<[**LicenseFeatureUpdateDto**](LicenseFeatureUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

