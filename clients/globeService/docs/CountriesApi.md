# \CountriesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_countries**](CountriesApi.md#count_countries) | **GET** /api/v2/GlobeService/Countries/Count | Count countries
[**get_all_countries**](CountriesApi.md#get_all_countries) | **GET** /api/v2/GlobeService/Countries | Get all countries
[**get_calling_codes_by_country_id_async**](CountriesApi.md#get_calling_codes_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/CallingCodes | Get calling codes for a country
[**get_cities_by_country_state_id_async**](CountriesApi.md#get_cities_by_country_state_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States/{countryStateId}/Cities | Get cities for a state
[**get_country_by_id**](CountriesApi.md#get_country_by_id) | **GET** /api/v2/GlobeService/Countries/{countryId} | Get country by ID
[**get_country_state_by_id_async**](CountriesApi.md#get_country_state_by_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States/{countryStateId} | Get state by ID
[**get_country_states_async**](CountriesApi.md#get_country_states_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/States | Get states for a country
[**get_enabled_currencies_by_country_id_async**](CountriesApi.md#get_enabled_currencies_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/Currencies | Get currencies for a country
[**get_time_zones_by_country_id_async**](CountriesApi.md#get_time_zones_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/Timezones | Get timezones for a country
[**get_top_level_domains_by_country_id_async**](CountriesApi.md#get_top_level_domains_by_country_id_async) | **GET** /api/v2/GlobeService/Countries/{countryId}/TopLevelDomains | Get top-level domains for a country
[**search_countries_by_name_async**](CountriesApi.md#search_countries_by_name_async) | **GET** /api/v2/GlobeService/Countries/Search | Search countries by name



## count_countries

> models::Int32Envelope count_countries(api_version, x_api_version)
Count countries

Returns the total number of countries, with optional OData filtering.

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
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_countries

> models::CountryDtoListEnvelope get_all_countries(api_version, x_api_version)
Get all countries

Retrieves a list of all countries with optional OData pagination and filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryDtoListEnvelope**](CountryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_calling_codes_by_country_id_async

> models::CountryCallingCodeDtoListEnvelope get_calling_codes_by_country_id_async(country_id, api_version, x_api_version)
Get calling codes for a country

Retrieves the list of international telephone calling codes associated with the specified country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryCallingCodeDtoListEnvelope**](CountryCallingCodeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cities_by_country_state_id_async

> models::CityDtoListEnvelope get_cities_by_country_state_id_async(country_state_id, country_id, api_version, x_api_version)
Get cities for a state

Retrieves the list of cities belonging to the specified state or province.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_state_id** | **String** |  | [required] |
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CityDtoListEnvelope**](CityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_country_by_id

> models::CountryDtoEnvelope get_country_by_id(country_id, api_version, x_api_version)
Get country by ID

Retrieves a single country by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryDtoEnvelope**](CountryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_country_state_by_id_async

> models::CountryStateDtoEnvelope get_country_state_by_id_async(country_state_id, country_id, api_version, x_api_version)
Get state by ID

Retrieves a single state or province by its unique identifier within a country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_state_id** | **String** |  | [required] |
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryStateDtoEnvelope**](CountryStateDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_country_states_async

> models::CountryStateDtoListEnvelope get_country_states_async(country_id, api_version, x_api_version)
Get states for a country

Retrieves the list of states or provinces belonging to the specified country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryStateDtoListEnvelope**](CountryStateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enabled_currencies_by_country_id_async

> models::CurrencyDtoListEnvelope get_enabled_currencies_by_country_id_async(country_id, api_version, x_api_version)
Get currencies for a country

Retrieves the list of enabled currencies for the specified country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CurrencyDtoListEnvelope**](CurrencyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_time_zones_by_country_id_async

> models::TimezoneDtoListEnvelope get_time_zones_by_country_id_async(country_id, api_version, x_api_version)
Get timezones for a country

Retrieves the list of timezones associated with the specified country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TimezoneDtoListEnvelope**](TimezoneDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_top_level_domains_by_country_id_async

> models::CountryTopLevelDomainDtoListEnvelope get_top_level_domains_by_country_id_async(country_id, api_version, x_api_version)
Get top-level domains for a country

Retrieves the list of internet top-level domains (TLDs) associated with the specified country.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryTopLevelDomainDtoListEnvelope**](CountryTopLevelDomainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_countries_by_name_async

> models::CountryDtoListEnvelope search_countries_by_name_async(country_name, api_version, x_api_version)
Search countries by name

Searches for countries whose name matches the specified search term.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**country_name** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CountryDtoListEnvelope**](CountryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

