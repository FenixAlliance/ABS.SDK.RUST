# \SupportEntitlementsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_entitlement_async**](SupportEntitlementsApi.md#create_support_entitlement_async) | **POST** /api/v2/SupportService/SupportEntitlements | Create a new support entitlement
[**delete_support_entitlement_async**](SupportEntitlementsApi.md#delete_support_entitlement_async) | **DELETE** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Delete a support entitlement
[**get_support_entitlement_async**](SupportEntitlementsApi.md#get_support_entitlement_async) | **GET** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Retrieve a support entitlement by ID
[**get_support_entitlements_async**](SupportEntitlementsApi.md#get_support_entitlements_async) | **GET** /api/v2/SupportService/SupportEntitlements | Retrieve a list of support entitlements
[**get_support_entitlements_count_async**](SupportEntitlementsApi.md#get_support_entitlements_count_async) | **GET** /api/v2/SupportService/SupportEntitlements/Count | Get the count of support entitlements
[**update_support_entitlement_async**](SupportEntitlementsApi.md#update_support_entitlement_async) | **PUT** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Update a support entitlement



## create_support_entitlement_async

> models::EmptyEnvelope create_support_entitlement_async(tenant_id, api_version, x_api_version, support_entitlement_create_dto)
Create a new support entitlement

Creates a new support entitlement for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_entitlement_create_dto** | Option<[**SupportEntitlementCreateDto**](SupportEntitlementCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_entitlement_async

> models::EmptyEnvelope delete_support_entitlement_async(tenant_id, support_entitlement_id, api_version, x_api_version)
Delete a support entitlement

Deletes a support entitlement by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_entitlement_id** | **uuid::Uuid** |  | [required] |
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


## get_support_entitlement_async

> models::SupportEntitlementDtoEnvelope get_support_entitlement_async(tenant_id, support_entitlement_id, api_version, x_api_version)
Retrieve a support entitlement by ID

Retrieves a single support entitlement by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_entitlement_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportEntitlementDtoEnvelope**](SupportEntitlementDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_entitlements_async

> models::SupportEntitlementDtoListEnvelope get_support_entitlements_async(tenant_id, api_version, x_api_version)
Retrieve a list of support entitlements

Retrieves a list of support entitlements for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportEntitlementDtoListEnvelope**](SupportEntitlementDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_entitlements_count_async

> models::Int32Envelope get_support_entitlements_count_async(tenant_id, api_version, x_api_version)
Get the count of support entitlements

Returns the total count of support entitlements for the specified tenant with OData query support.

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


## update_support_entitlement_async

> models::EmptyEnvelope update_support_entitlement_async(tenant_id, support_entitlement_id, api_version, x_api_version, support_entitlement_update_dto)
Update a support entitlement

Updates an existing support entitlement by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_entitlement_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_entitlement_update_dto** | Option<[**SupportEntitlementUpdateDto**](SupportEntitlementUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

