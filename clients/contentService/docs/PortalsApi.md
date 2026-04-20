# \PortalsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_portals_async**](PortalsApi.md#count_portals_async) | **GET** /api/v2/ContentService/Portals/Count | Count portals
[**create_web_portal_async**](PortalsApi.md#create_web_portal_async) | **POST** /api/v2/ContentService/Portals | Create a new web portal
[**delete_web_portal_async**](PortalsApi.md#delete_web_portal_async) | **DELETE** /api/v2/ContentService/Portals/{portalId} | Delete a web portal
[**get_current_web_portal_async**](PortalsApi.md#get_current_web_portal_async) | **GET** /api/v2/ContentService/Portals/Current | Get the current portal
[**get_current_web_portal_options_async**](PortalsApi.md#get_current_web_portal_options_async) | **GET** /api/v2/ContentService/Portals/Current/Options | Get the current portal's options
[**get_portals_async**](PortalsApi.md#get_portals_async) | **GET** /api/v2/ContentService/Portals | Get portals
[**get_root_web_portal_async**](PortalsApi.md#get_root_web_portal_async) | **GET** /api/v2/ContentService/Portals/Root | Get the root portal
[**get_web_portal_by_id_async**](PortalsApi.md#get_web_portal_by_id_async) | **GET** /api/v2/ContentService/Portals/{portalId} | Get a web portal by its ID
[**get_web_portal_options_async**](PortalsApi.md#get_web_portal_options_async) | **GET** /api/v2/ContentService/Portals/{portalId}/Options | Get a web portal's options by its ID
[**get_web_portal_settings_async**](PortalsApi.md#get_web_portal_settings_async) | **GET** /api/v2/ContentService/Portals/{portalId}/Settings | Get a web portal's settings by its ID
[**initialize_current_web_portal_async**](PortalsApi.md#initialize_current_web_portal_async) | **POST** /api/v2/ContentService/Portals/Initialize | Initialize the current portal
[**patch_web_portal_async**](PortalsApi.md#patch_web_portal_async) | **PATCH** /api/v2/ContentService/Portals/{portalId} | Partially update a web portal
[**search_web_portal_async**](PortalsApi.md#search_web_portal_async) | **GET** /api/v2/ContentService/Portals/Search | Search for a portal by its domain
[**update_web_portal_async**](PortalsApi.md#update_web_portal_async) | **PUT** /api/v2/ContentService/Portals/{portalId} | Update an existing web portal



## count_portals_async

> models::Int32Envelope count_portals_async(tenant_id, api_version, x_api_version)
Count portals

Counts all portals for the specified tenant.

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


## create_web_portal_async

> models::EmptyEnvelope create_web_portal_async(tenant_id, api_version, x_api_version, web_portal_create_dto)
Create a new web portal

Create a new web portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_portal_create_dto** | Option<[**WebPortalCreateDto**](WebPortalCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_web_portal_async

> models::EmptyEnvelope delete_web_portal_async(tenant_id, portal_id, api_version, x_api_version)
Delete a web portal

Delete a web portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**portal_id** | **uuid::Uuid** |  | [required] |
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


## get_current_web_portal_async

> models::WebPortalDtoEnvelope get_current_web_portal_async(api_version, x_api_version)
Get the current portal

Get the current portal of the this server instance

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_web_portal_options_async

> models::PortalOptionsEnvelope get_current_web_portal_options_async(api_version, x_api_version)
Get the current portal's options

Get the current portal's options for the current user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PortalOptionsEnvelope**](PortalOptionsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_portals_async

> models::WebPortalDtoListEnvelope get_portals_async(tenant_id, api_version, x_api_version)
Get portals

Retrieves all portals for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoListEnvelope**](WebPortalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_root_web_portal_async

> models::WebPortalDtoEnvelope get_root_web_portal_async(api_version, x_api_version)
Get the root portal

Get the root portal of the this server instance

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_portal_by_id_async

> models::WebPortalDtoEnvelope get_web_portal_by_id_async(portal_id, api_version, x_api_version)
Get a web portal by its ID

Get a web portal by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_portal_options_async

> models::PortalOptionsEnvelope get_web_portal_options_async(portal_id, api_version, x_api_version)
Get a web portal's options by its ID

Get a web portal's options by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PortalOptionsEnvelope**](PortalOptionsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_web_portal_settings_async

> models::PortalSettingsEnvelope get_web_portal_settings_async(portal_id, api_version, x_api_version)
Get a web portal's settings by its ID

Get a web portal's settings by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**portal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PortalSettingsEnvelope**](PortalSettingsEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## initialize_current_web_portal_async

> models::WebPortalDtoEnvelope initialize_current_web_portal_async(api_version, x_api_version)
Initialize the current portal

Initialize the current portal for the current user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_web_portal_async

> models::EmptyEnvelope patch_web_portal_async(tenant_id, portal_id, api_version, x_api_version, operation)
Partially update a web portal

Partially update a web portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**portal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## search_web_portal_async

> models::WebPortalDtoEnvelope search_web_portal_async(domain, api_version, x_api_version)
Search for a portal by its domain

Search for a portal by its domain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WebPortalDtoEnvelope**](WebPortalDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_web_portal_async

> models::EmptyEnvelope update_web_portal_async(tenant_id, portal_id, api_version, x_api_version, web_portal_update_dto)
Update an existing web portal

Update an existing web portal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**portal_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**web_portal_update_dto** | Option<[**WebPortalUpdateDto**](WebPortalUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

