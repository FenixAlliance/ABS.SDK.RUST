# \LanguagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_languages_async**](LanguagesApi.md#count_languages_async) | **GET** /api/v2/GlobeService/Languages/Count | Count languages
[**get_language_by_id_async**](LanguagesApi.md#get_language_by_id_async) | **GET** /api/v2/GlobeService/Languages/{languageId} | Get language by ID
[**get_languages_async**](LanguagesApi.md#get_languages_async) | **GET** /api/v2/GlobeService/Languages | Get all languages



## count_languages_async

> models::Int32Envelope count_languages_async(api_version, x_api_version)
Count languages

Returns the total number of supported languages, with optional OData filtering.

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


## get_language_by_id_async

> models::CountryLanguageDtoEnvelope get_language_by_id_async(language_id, api_version, x_api_version)
Get language by ID

Retrieves a single language by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**language_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryLanguageDtoEnvelope**](CountryLanguageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_languages_async

> models::CountryLanguageDtoListEnvelope get_languages_async(api_version, x_api_version)
Get all languages

Retrieves the list of all supported languages with optional OData pagination and filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryLanguageDtoListEnvelope**](CountryLanguageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

