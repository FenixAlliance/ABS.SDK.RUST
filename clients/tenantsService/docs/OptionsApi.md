# \OptionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_option**](OptionsApi.md#create_tenant_option) | **POST** /api/v2/TenantsService/Options | Create a new tenant option
[**delete_tenant_option**](OptionsApi.md#delete_tenant_option) | **DELETE** /api/v2/TenantsService/Options/{optionId} | Delete a tenant option
[**get_tenant_option_by_id**](OptionsApi.md#get_tenant_option_by_id) | **GET** /api/v2/TenantsService/Options/{optionId} | Retrieve a single tenant option by its ID
[**get_tenant_option_by_key**](OptionsApi.md#get_tenant_option_by_key) | **GET** /api/v2/TenantsService/Options/Key/{key} | Retrieve a single tenant option by its key
[**get_tenant_options**](OptionsApi.md#get_tenant_options) | **GET** /api/v2/TenantsService/Options | Retrieve a list of tenant options
[**get_tenant_options_count**](OptionsApi.md#get_tenant_options_count) | **GET** /api/v2/TenantsService/Options/Count | Get the count of tenant options
[**update_tenant_option**](OptionsApi.md#update_tenant_option) | **PUT** /api/v2/TenantsService/Options/{optionId} | Update a tenant option
[**upsert_tenant_option**](OptionsApi.md#upsert_tenant_option) | **PUT** /api/v2/TenantsService/Options/Upsert/{key} | Create or update a tenant option by key



## create_tenant_option

> models::EmptyEnvelope create_tenant_option(tenant_id, key, portal_id, api_version, x_api_version, option_create_dto)
Create a new tenant option

Create a new tenant option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**option_create_dto** | Option<[**OptionCreateDto**](OptionCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_option

> models::EmptyEnvelope delete_tenant_option(tenant_id, option_id, api_version, x_api_version)
Delete a tenant option

Delete a tenant option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_option_by_id

> models::OptionDtoEnvelope get_tenant_option_by_id(tenant_id, option_id, api_version, x_api_version)
Retrieve a single tenant option by its ID

Retrieve a single tenant option by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_option_by_key

> models::OptionDtoEnvelope get_tenant_option_by_key(tenant_id, key, portal_id, api_version, x_api_version)
Retrieve a single tenant option by its key

Retrieve a single tenant option by its key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_options

> models::OptionDtoListEnvelope get_tenant_options(tenant_id, portal_id, api_version, x_api_version)
Retrieve a list of tenant options

Retrieve a list of tenant options

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OptionDtoListEnvelope**](OptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_options_count

> models::Int32Envelope get_tenant_options_count(tenant_id, portal_id, api_version, x_api_version)
Get the count of tenant options

Get the count of tenant options

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
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


## update_tenant_option

> models::EmptyEnvelope update_tenant_option(tenant_id, option_id, api_version, x_api_version, option_update_dto)
Update a tenant option

Update a tenant option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**option_update_dto** | Option<[**OptionUpdateDto**](OptionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upsert_tenant_option

> models::EmptyEnvelope upsert_tenant_option(tenant_id, key, portal_id, api_version, x_api_version, option_update_dto)
Create or update a tenant option by key

Create or update a tenant option by key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**option_update_dto** | Option<[**OptionUpdateDto**](OptionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

