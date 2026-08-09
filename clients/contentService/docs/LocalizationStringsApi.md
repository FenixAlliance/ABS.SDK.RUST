# \LocalizationStringsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_localization_strings_async**](LocalizationStringsApi.md#count_localization_strings_async) | **GET** /api/v2/ContentService/LocalizationStrings/Count | Count localization strings
[**create_localization_string_async**](LocalizationStringsApi.md#create_localization_string_async) | **POST** /api/v2/ContentService/LocalizationStrings | Create a localization string
[**delete_localization_string_async**](LocalizationStringsApi.md#delete_localization_string_async) | **DELETE** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Delete a localization string
[**get_localization_string_by_id_async**](LocalizationStringsApi.md#get_localization_string_by_id_async) | **GET** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Get localization string by ID
[**get_localization_strings_async**](LocalizationStringsApi.md#get_localization_strings_async) | **GET** /api/v2/ContentService/LocalizationStrings | Get localization strings
[**update_localization_string_async**](LocalizationStringsApi.md#update_localization_string_async) | **PUT** /api/v2/ContentService/LocalizationStrings/{localizationStringId} | Update a localization string



## count_localization_strings_async

> models::Int32Envelope count_localization_strings_async(tenant_id, api_version, x_api_version, localization_string_dto_collection_query_parameters)
Count localization strings

Counts all localization strings for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**localization_string_dto_collection_query_parameters** | Option<[**LocalizationStringDtoCollectionQueryParameters**](LocalizationStringDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_localization_string_async

> models::EmptyEnvelope create_localization_string_async(tenant_id, localization_string_create_dto, api_version, x_api_version)
Create a localization string

Creates a new localization string for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**localization_string_create_dto** | [**LocalizationStringCreateDto**](LocalizationStringCreateDto.md) |  | [required] |
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


## delete_localization_string_async

> models::EmptyEnvelope delete_localization_string_async(tenant_id, localization_string_id, api_version, x_api_version)
Delete a localization string

Deletes a localization string for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**localization_string_id** | **uuid::Uuid** |  | [required] |
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


## get_localization_string_by_id_async

> models::LocalizationStringDtoEnvelope get_localization_string_by_id_async(tenant_id, localization_string_id, api_version, x_api_version)
Get localization string by ID

Retrieves a specific localization string by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**localization_string_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LocalizationStringDtoEnvelope**](LocalizationStringDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_localization_strings_async

> models::LocalizationStringDtoListEnvelope get_localization_strings_async(tenant_id, api_version, x_api_version, localization_string_dto_collection_query_parameters)
Get localization strings

Retrieves all localization strings for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**localization_string_dto_collection_query_parameters** | Option<[**LocalizationStringDtoCollectionQueryParameters**](LocalizationStringDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::LocalizationStringDtoListEnvelope**](LocalizationStringDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_localization_string_async

> models::EmptyEnvelope update_localization_string_async(tenant_id, localization_string_id, localization_string_update_dto, api_version, x_api_version)
Update a localization string

Updates an existing localization string for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**localization_string_id** | **uuid::Uuid** |  | [required] |
**localization_string_update_dto** | [**LocalizationStringUpdateDto**](LocalizationStringUpdateDto.md) |  | [required] |
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

