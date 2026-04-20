# \IndustriesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_industry**](IndustriesApi.md#create_tenant_industry) | **POST** /api/v2/TenantsService/Industries | Create a new tenant industry
[**delete_tenant_industry**](IndustriesApi.md#delete_tenant_industry) | **DELETE** /api/v2/TenantsService/Industries/{tenantIndustryId} | Delete a tenant industry
[**get_tenant_industries**](IndustriesApi.md#get_tenant_industries) | **GET** /api/v2/TenantsService/Industries | Retrieve a list of tenant industries
[**get_tenant_industries_count**](IndustriesApi.md#get_tenant_industries_count) | **GET** /api/v2/TenantsService/Industries/Count | Get the count of tenant industries
[**get_tenant_industry_by_id**](IndustriesApi.md#get_tenant_industry_by_id) | **GET** /api/v2/TenantsService/Industries/{tenantIndustryId} | Retrieve a single tenant industry by its ID
[**update_tenant_industry**](IndustriesApi.md#update_tenant_industry) | **PUT** /api/v2/TenantsService/Industries/{tenantIndustryId} | Update a tenant industry



## create_tenant_industry

> models::EmptyEnvelope create_tenant_industry(tenant_id, api_version, x_api_version, tenant_industry_create_dto)
Create a new tenant industry

Create a new tenant industry

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_industry_create_dto** | Option<[**TenantIndustryCreateDto**](TenantIndustryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_industry

> models::EmptyEnvelope delete_tenant_industry(tenant_id, tenant_industry_id, api_version, x_api_version)
Delete a tenant industry

Delete a tenant industry

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_industry_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_industries

> models::TenantIndustryDtoListEnvelope get_tenant_industries(tenant_id, api_version, x_api_version)
Retrieve a list of tenant industries

Retrieve a list of tenant industries

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantIndustryDtoListEnvelope**](TenantIndustryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_industries_count

> models::Int32Envelope get_tenant_industries_count(tenant_id, api_version, x_api_version)
Get the count of tenant industries

Get the count of tenant industries

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


## get_tenant_industry_by_id

> models::TenantIndustryDtoEnvelope get_tenant_industry_by_id(tenant_id, tenant_industry_id, api_version, x_api_version)
Retrieve a single tenant industry by its ID

Retrieve a single tenant industry by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_industry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantIndustryDtoEnvelope**](TenantIndustryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tenant_industry

> models::EmptyEnvelope update_tenant_industry(tenant_id, tenant_industry_id, api_version, x_api_version, tenant_industry_update_dto)
Update a tenant industry

Update a tenant industry

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_industry_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_industry_update_dto** | Option<[**TenantIndustryUpdateDto**](TenantIndustryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

