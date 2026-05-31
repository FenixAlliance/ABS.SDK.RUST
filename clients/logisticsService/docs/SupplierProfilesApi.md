# \SupplierProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_supplier_profile_async**](SupplierProfilesApi.md#create_supplier_profile_async) | **POST** /api/v2/LogisticsService/SupplierProfiles | Create a supplier profile
[**delete_supplier_profile_async**](SupplierProfilesApi.md#delete_supplier_profile_async) | **DELETE** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Delete a supplier profile
[**get_supplier_profile_by_id_async**](SupplierProfilesApi.md#get_supplier_profile_by_id_async) | **GET** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Get supplier profile by ID
[**get_supplier_profiles_async**](SupplierProfilesApi.md#get_supplier_profiles_async) | **GET** /api/v2/LogisticsService/SupplierProfiles | Get all supplier profiles
[**get_supplier_profiles_count_async**](SupplierProfilesApi.md#get_supplier_profiles_count_async) | **GET** /api/v2/LogisticsService/SupplierProfiles/Count | Get supplier profiles count
[**update_supplier_profile_async**](SupplierProfilesApi.md#update_supplier_profile_async) | **PUT** /api/v2/LogisticsService/SupplierProfiles/{supplierProfileId} | Update a supplier profile



## create_supplier_profile_async

> models::EmptyEnvelope create_supplier_profile_async(tenant_id, api_version, x_api_version, supplier_profile_create_dto)
Create a supplier profile

Creates a new supplier profile for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**supplier_profile_create_dto** | Option<[**SupplierProfileCreateDto**](SupplierProfileCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_supplier_profile_async

> models::EmptyEnvelope delete_supplier_profile_async(tenant_id, supplier_profile_id, api_version, x_api_version)
Delete a supplier profile

Deletes a supplier profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**supplier_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_supplier_profile_by_id_async

> models::SupplierProfileDtoEnvelope get_supplier_profile_by_id_async(tenant_id, supplier_profile_id, api_version, x_api_version)
Get supplier profile by ID

Retrieves a specific supplier profile by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**supplier_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupplierProfileDtoEnvelope**](SupplierProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_supplier_profiles_async

> models::SupplierProfileDtoListEnvelope get_supplier_profiles_async(tenant_id, api_version, x_api_version)
Get all supplier profiles

Retrieves all supplier profiles for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupplierProfileDtoListEnvelope**](SupplierProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_supplier_profiles_count_async

> models::Int32Envelope get_supplier_profiles_count_async(tenant_id, api_version, x_api_version)
Get supplier profiles count

Returns the count of supplier profiles for the specified tenant.

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


## update_supplier_profile_async

> models::EmptyEnvelope update_supplier_profile_async(tenant_id, supplier_profile_id, api_version, x_api_version, supplier_profile_update_dto)
Update a supplier profile

Updates an existing supplier profile.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**supplier_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**supplier_profile_update_dto** | Option<[**SupplierProfileUpdateDto**](SupplierProfileUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

