# \CapabilitiesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_capabilities_async**](CapabilitiesApi.md#get_capabilities_async) | **GET** /api/v2/IntelligenceService/Capabilities | Get the annotated capability catalog
[**get_capabilities_count_async**](CapabilitiesApi.md#get_capabilities_count_async) | **GET** /api/v2/IntelligenceService/Capabilities/Count | Get the capability catalog count
[**get_capability_by_key_async**](CapabilitiesApi.md#get_capability_by_key_async) | **GET** /api/v2/IntelligenceService/Capabilities/{key} | Get a capability by key



## get_capabilities_async

> models::CapabilityDtoListEnvelope get_capabilities_async(tenant_id, surface, api_version, x_api_version)
Get the annotated capability catalog

Retrieves the full governed-capability catalog for the specified tenant, optionally narrowed to a single execution surface. Every capability is returned with an Available flag (and a DeniedReason when not available) so callers render disabled-with-reason instead of hiding; entitlement is computed server-side.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**surface** | Option<**String**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CapabilityDtoListEnvelope**](CapabilityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_capabilities_count_async

> models::Int32Envelope get_capabilities_count_async(tenant_id, surface, api_version, x_api_version)
Get the capability catalog count

Returns the number of governed capabilities in the catalog for the specified tenant — the surface-matching total that mirrors the list route's returned-set size (entitled or not), honouring the same optional surface narrowing.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**surface** | Option<**String**> |  |  |
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


## get_capability_by_key_async

> models::CapabilityDtoEnvelope get_capability_by_key_async(tenant_id, key, api_version, x_api_version)
Get a capability by key

Retrieves a single governed capability by its stable, dotted key, stamped with the Available / DeniedReason entitlement flag. Returns 404 only when the capability does not exist; an existing capability the actor is not entitled to run is returned annotated as unavailable, not hidden.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CapabilityDtoEnvelope**](CapabilityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

