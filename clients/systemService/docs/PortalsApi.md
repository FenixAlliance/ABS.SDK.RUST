# \PortalsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_system_portal**](PortalsApi.md#create_system_portal) | **POST** /api/v2/SystemService/Portals | Create a new system portal
[**delete_system_portal**](PortalsApi.md#delete_system_portal) | **DELETE** /api/v2/SystemService/Portals/{portalId} | Delete a system portal
[**get_system_portal_by_id**](PortalsApi.md#get_system_portal_by_id) | **GET** /api/v2/SystemService/Portals/{portalId} | Retrieve a single system portal by its ID
[**get_system_portals**](PortalsApi.md#get_system_portals) | **GET** /api/v2/SystemService/Portals | Retrieve a list of system portals
[**get_system_portals_count**](PortalsApi.md#get_system_portals_count) | **GET** /api/v2/SystemService/Portals/Count | Get the count of system portals
[**update_system_portal**](PortalsApi.md#update_system_portal) | **PUT** /api/v2/SystemService/Portals/{portalId} | Update a system portal



## create_system_portal

> models::EmptyEnvelope create_system_portal(api_version, x_api_version, web_portal_create_dto)
Create a new system portal

Create a new web portal in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## delete_system_portal

> models::EmptyEnvelope delete_system_portal(portal_id, api_version, x_api_version)
Delete a system portal

Delete a web portal from the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_system_portal_by_id

> models::WebPortalDtoEnvelope get_system_portal_by_id(portal_id, api_version, x_api_version)
Retrieve a single system portal by its ID

Retrieve a single system portal by its ID

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


## get_system_portals

> models::WebPortalDtoListEnvelope get_system_portals(api_version, x_api_version)
Retrieve a list of system portals

Retrieve a list of all web portals in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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


## get_system_portals_count

> models::Int32Envelope get_system_portals_count(api_version, x_api_version)
Get the count of system portals

Get the count of all web portals in the system

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


## update_system_portal

> models::EmptyEnvelope update_system_portal(portal_id, api_version, x_api_version, web_portal_update_dto)
Update a system portal

Update an existing web portal in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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

