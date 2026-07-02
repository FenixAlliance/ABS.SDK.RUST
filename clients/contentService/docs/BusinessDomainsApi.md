# \BusinessDomainsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_business_domain_async**](BusinessDomainsApi.md#create_business_domain_async) | **POST** /api/v2/ContentService/BusinessDomains | Register a business domain
[**delete_business_domain_async**](BusinessDomainsApi.md#delete_business_domain_async) | **DELETE** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Delete a business domain
[**get_business_domain_by_id_async**](BusinessDomainsApi.md#get_business_domain_by_id_async) | **GET** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Get business domain by ID
[**get_business_domains_async**](BusinessDomainsApi.md#get_business_domains_async) | **GET** /api/v2/ContentService/BusinessDomains | Get business domains
[**get_business_domains_count_async**](BusinessDomainsApi.md#get_business_domains_count_async) | **GET** /api/v2/ContentService/BusinessDomains/Count | Get business domains count
[**update_business_domain_async**](BusinessDomainsApi.md#update_business_domain_async) | **PUT** /api/v2/ContentService/BusinessDomains/{businessDomainId} | Update a business domain
[**verify_business_domain_async**](BusinessDomainsApi.md#verify_business_domain_async) | **POST** /api/v2/ContentService/BusinessDomains/{businessDomainId}/Verify | Verify a business domain



## create_business_domain_async

> models::EmptyEnvelope create_business_domain_async(tenant_id, business_domain_create_dto, api_version, x_api_version)
Register a business domain

Registers a new (unverified) business domain for the tenant and issues a DNS TXT verification token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_domain_create_dto** | [**BusinessDomainCreateDto**](BusinessDomainCreateDto.md) |  | [required] |
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


## delete_business_domain_async

> models::EmptyEnvelope delete_business_domain_async(tenant_id, business_domain_id, api_version, x_api_version)
Delete a business domain

Removes a business domain from the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_domain_id** | **uuid::Uuid** |  | [required] |
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


## get_business_domain_by_id_async

> models::BusinessDomainDtoEnvelope get_business_domain_by_id_async(tenant_id, business_domain_id, api_version, x_api_version)
Get business domain by ID

Retrieves a specific business domain.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_domain_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessDomainDtoEnvelope**](BusinessDomainDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_domains_async

> models::BusinessDomainDtoListEnvelope get_business_domains_async(tenant_id, api_version, x_api_version)
Get business domains

Retrieves business domains for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessDomainDtoListEnvelope**](BusinessDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_domains_count_async

> models::Int32Envelope get_business_domains_count_async(tenant_id, api_version, x_api_version)
Get business domains count

Retrieves the count of business domains for the specified tenant.

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


## update_business_domain_async

> models::EmptyEnvelope update_business_domain_async(tenant_id, business_domain_id, business_domain_update_dto, api_version, x_api_version)
Update a business domain

Updates a business domain. Changing the host re-issues the verification token and clears verification.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_domain_id** | **uuid::Uuid** |  | [required] |
**business_domain_update_dto** | [**BusinessDomainUpdateDto**](BusinessDomainUpdateDto.md) |  | [required] |
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


## verify_business_domain_async

> models::EmptyEnvelope verify_business_domain_async(tenant_id, business_domain_id, api_version, x_api_version)
Verify a business domain

Checks the domain's DNS TXT records for the verification token and marks the domain verified.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_domain_id** | **uuid::Uuid** |  | [required] |
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

