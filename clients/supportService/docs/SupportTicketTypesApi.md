# \SupportTicketTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_ticket_type_async**](SupportTicketTypesApi.md#create_support_ticket_type_async) | **POST** /api/v2/SupportService/SupportTicketTypes | Create a new support ticket type
[**delete_support_ticket_type_async**](SupportTicketTypesApi.md#delete_support_ticket_type_async) | **DELETE** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Delete a support ticket type
[**get_support_ticket_type_async**](SupportTicketTypesApi.md#get_support_ticket_type_async) | **GET** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Retrieve a support ticket type by ID
[**get_support_ticket_types_async**](SupportTicketTypesApi.md#get_support_ticket_types_async) | **GET** /api/v2/SupportService/SupportTicketTypes | Retrieve a list of support ticket types
[**get_support_ticket_types_count_async**](SupportTicketTypesApi.md#get_support_ticket_types_count_async) | **GET** /api/v2/SupportService/SupportTicketTypes/Count | Get the count of support ticket types
[**update_support_ticket_type_async**](SupportTicketTypesApi.md#update_support_ticket_type_async) | **PUT** /api/v2/SupportService/SupportTicketTypes/{supportTicketTypeId} | Update a support ticket type



## create_support_ticket_type_async

> models::EmptyEnvelope create_support_ticket_type_async(tenant_id, api_version, x_api_version, support_ticket_type_create_dto)
Create a new support ticket type

Creates a new support ticket type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_type_create_dto** | Option<[**SupportTicketTypeCreateDto**](SupportTicketTypeCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_ticket_type_async

> models::EmptyEnvelope delete_support_ticket_type_async(tenant_id, support_ticket_type_id, api_version, x_api_version)
Delete a support ticket type

Deletes a support ticket type by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_type_id** | **uuid::Uuid** |  | [required] |
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


## get_support_ticket_type_async

> models::SupportTicketTypeDtoEnvelope get_support_ticket_type_async(tenant_id, support_ticket_type_id, api_version, x_api_version)
Retrieve a support ticket type by ID

Retrieves a single support ticket type by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketTypeDtoEnvelope**](SupportTicketTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_types_async

> models::SupportTicketTypeDtoListEnvelope get_support_ticket_types_async(tenant_id, api_version, x_api_version)
Retrieve a list of support ticket types

Retrieves a list of support ticket types for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketTypeDtoListEnvelope**](SupportTicketTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_types_count_async

> models::Int32Envelope get_support_ticket_types_count_async(tenant_id, api_version, x_api_version)
Get the count of support ticket types

Returns the total count of support ticket types for the specified tenant with OData query support.

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


## update_support_ticket_type_async

> models::EmptyEnvelope update_support_ticket_type_async(tenant_id, support_ticket_type_id, api_version, x_api_version, support_ticket_type_update_dto)
Update a support ticket type

Updates an existing support ticket type by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_type_update_dto** | Option<[**SupportTicketTypeUpdateDto**](SupportTicketTypeUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

