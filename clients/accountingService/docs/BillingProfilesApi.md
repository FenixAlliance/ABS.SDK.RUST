# \BillingProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_billing_profile_async**](BillingProfilesApi.md#create_billing_profile_async) | **POST** /api/v2/AccountingService/BillingProfiles | Creates a new billing profile
[**delete_billing_profile_async**](BillingProfilesApi.md#delete_billing_profile_async) | **DELETE** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Deletes a billing profile
[**get_billing_profile_by_id_async**](BillingProfilesApi.md#get_billing_profile_by_id_async) | **GET** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Gets a billing profile by id
[**get_billing_profiles_async**](BillingProfilesApi.md#get_billing_profiles_async) | **GET** /api/v2/AccountingService/BillingProfiles | Gets all billing profiles
[**get_billing_profiles_count_async**](BillingProfilesApi.md#get_billing_profiles_count_async) | **GET** /api/v2/AccountingService/BillingProfiles/Count | Gets the count of billing profiles
[**update_billing_profile_async**](BillingProfilesApi.md#update_billing_profile_async) | **PUT** /api/v2/AccountingService/BillingProfiles/{billingProfileId} | Updates an existing billing profile



## create_billing_profile_async

> models::EmptyEnvelope create_billing_profile_async(tenant_id, billing_profile_create_dto, api_version, x_api_version)
Creates a new billing profile

Adds a new billing profile record for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billing_profile_create_dto** | [**BillingProfileCreateDto**](BillingProfileCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_billing_profile_async

> models::EmptyEnvelope delete_billing_profile_async(tenant_id, billing_profile_id, api_version, x_api_version)
Deletes a billing profile

Removes a billing profile from the system using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billing_profile_id** | **uuid::Uuid** |  | [required] |
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


## get_billing_profile_by_id_async

> models::BillingProfileDtoEnvelope get_billing_profile_by_id_async(tenant_id, billing_profile_id, api_version, x_api_version)
Gets a billing profile by id

Retrieves a specific billing profile using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billing_profile_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillingProfileDtoEnvelope**](BillingProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_billing_profiles_async

> models::BillingProfileDtoIReadOnlyListEnvelope get_billing_profiles_async(tenant_id, api_version, x_api_version)
Gets all billing profiles

Fetches all billing profiles for a tenant with support for OData queries.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BillingProfileDtoIReadOnlyListEnvelope**](BillingProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_billing_profiles_count_async

> models::Int32Envelope get_billing_profiles_count_async(tenant_id, api_version, x_api_version)
Gets the count of billing profiles

Returns the number of billing profiles for a tenant, supporting OData filtering.

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


## update_billing_profile_async

> models::EmptyEnvelope update_billing_profile_async(tenant_id, billing_profile_id, billing_profile_update_dto, api_version, x_api_version)
Updates an existing billing profile

Modifies an existing billing profile using the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**billing_profile_id** | **uuid::Uuid** |  | [required] |
**billing_profile_update_dto** | [**BillingProfileUpdateDto**](BillingProfileUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

