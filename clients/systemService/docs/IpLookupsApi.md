# \IpLookupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_system_ip_lookup**](IpLookupsApi.md#delete_system_ip_lookup) | **DELETE** /api/v2/SystemService/IPLookups/{ipLookupId} | Delete a system IP lookup
[**get_system_ip_lookup_by_id**](IpLookupsApi.md#get_system_ip_lookup_by_id) | **GET** /api/v2/SystemService/IPLookups/{ipLookupId} | Retrieve a single system IP lookup by its ID
[**get_system_ip_lookups**](IpLookupsApi.md#get_system_ip_lookups) | **GET** /api/v2/SystemService/IPLookups | Retrieve a list of system IP lookups
[**get_system_ip_lookups_count**](IpLookupsApi.md#get_system_ip_lookups_count) | **GET** /api/v2/SystemService/IPLookups/Count | Get the count of system IP lookups



## delete_system_ip_lookup

> models::EmptyEnvelope delete_system_ip_lookup(ip_lookup_id, api_version, x_api_version)
Delete a system IP lookup

Delete a system IP lookup by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ip_lookup_id** | **uuid::Uuid** |  | [required] |
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


## get_system_ip_lookup_by_id

> models::IpLookupDtoEnvelope get_system_ip_lookup_by_id(ip_lookup_id, api_version, x_api_version)
Retrieve a single system IP lookup by its ID

Retrieve a single system IP lookup by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ip_lookup_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::IpLookupDtoEnvelope**](IPLookupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_ip_lookups

> models::IpLookupDtoListEnvelope get_system_ip_lookups(api_version, x_api_version)
Retrieve a list of system IP lookups

Retrieve a list of all IP lookups in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::IpLookupDtoListEnvelope**](IPLookupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_ip_lookups_count

> models::Int32Envelope get_system_ip_lookups_count(api_version, x_api_version)
Get the count of system IP lookups

Get the count of all IP lookups in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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

