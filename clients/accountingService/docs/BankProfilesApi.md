# \BankProfilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_bank_profiles**](BankProfilesApi.md#get_bank_profiles) | **GET** /api/v2/AccountingService/BankProfiles | Get all bank profiles for a tenant
[**get_bank_profiles_count**](BankProfilesApi.md#get_bank_profiles_count) | **GET** /api/v2/AccountingService/BankProfiles/Count | Get bank profiles count



## get_bank_profiles

> models::BankProfileDtoListEnvelope get_bank_profiles(tenant_id, api_version, x_api_version)
Get all bank profiles for a tenant

Retrieves all bank profiles for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BankProfileDtoListEnvelope**](BankProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_bank_profiles_count

> models::Int32Envelope get_bank_profiles_count(tenant_id, api_version, x_api_version)
Get bank profiles count

Returns the count of bank profiles for the specified tenant.

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

