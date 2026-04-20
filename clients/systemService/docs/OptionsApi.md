# \OptionsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_system_option**](OptionsApi.md#create_system_option) | **POST** /api/v2/SystemService/Options | Create a new system option
[**delete_system_option**](OptionsApi.md#delete_system_option) | **DELETE** /api/v2/SystemService/Options/{optionId} | Delete a system option
[**get_system_option_by_id**](OptionsApi.md#get_system_option_by_id) | **GET** /api/v2/SystemService/Options/{optionId} | Retrieve a single system option by its ID
[**get_system_option_by_key**](OptionsApi.md#get_system_option_by_key) | **GET** /api/v2/SystemService/Options/Key/{key} | Retrieve a single system option by its key
[**get_system_options**](OptionsApi.md#get_system_options) | **GET** /api/v2/SystemService/Options | Retrieve a list of system options
[**get_system_options_count**](OptionsApi.md#get_system_options_count) | **GET** /api/v2/SystemService/Options/Count | Get the count of system options
[**update_system_option**](OptionsApi.md#update_system_option) | **PUT** /api/v2/SystemService/Options/{optionId} | Update a system option
[**upsert_system_option**](OptionsApi.md#upsert_system_option) | **PUT** /api/v2/SystemService/Options/Upsert/{key} | Create or update a system option by key



## create_system_option

> models::EmptyEnvelope create_system_option(key, portal_id, api_version, x_api_version, option_create_dto)
Create a new system option

Create a new system option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## delete_system_option

> models::EmptyEnvelope delete_system_option(option_id, api_version, x_api_version)
Delete a system option

Delete a system option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_system_option_by_id

> models::OptionDtoEnvelope get_system_option_by_id(option_id, api_version, x_api_version)
Retrieve a single system option by its ID

Retrieve a single system option by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_system_option_by_key

> models::OptionDtoEnvelope get_system_option_by_key(portal_id, key, api_version, x_api_version)
Retrieve a single system option by its key

Retrieve a single system option by its key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
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


## get_system_options

> models::OptionDtoListEnvelope get_system_options(portal_id, api_version, x_api_version)
Retrieve a list of system options

Retrieve a list of system options for a portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
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


## get_system_options_count

> models::Int32Envelope get_system_options_count(portal_id, api_version, x_api_version)
Get the count of system options

Get the count of system options for a portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
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


## update_system_option

> models::EmptyEnvelope update_system_option(option_id, api_version, x_api_version, option_update_dto)
Update a system option

Update a system option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## upsert_system_option

> models::EmptyEnvelope upsert_system_option(key, portal_id, api_version, x_api_version, option_update_dto)
Create or update a system option by key

Create or update a system option by key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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

