# \SupportTicketPrioritiesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#create_support_ticket_priority_async) | **POST** /api/v2/SupportService/SupportTicketPriorities | Create a new support ticket priority
[**delete_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#delete_support_ticket_priority_async) | **DELETE** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Delete a support ticket priority
[**get_support_ticket_priorities_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priorities_async) | **GET** /api/v2/SupportService/SupportTicketPriorities | Retrieve a list of support ticket priorities
[**get_support_ticket_priorities_count_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priorities_count_async) | **GET** /api/v2/SupportService/SupportTicketPriorities/Count | Get the count of support ticket priorities
[**get_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#get_support_ticket_priority_async) | **GET** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Retrieve a support ticket priority by ID
[**update_support_ticket_priority_async**](SupportTicketPrioritiesApi.md#update_support_ticket_priority_async) | **PUT** /api/v2/SupportService/SupportTicketPriorities/{supportTicketPriorityId} | Update a support ticket priority



## create_support_ticket_priority_async

> models::EmptyEnvelope create_support_ticket_priority_async(tenant_id, api_version, x_api_version, support_ticket_priority_create_dto)
Create a new support ticket priority

Creates a new support ticket priority for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_priority_create_dto** | Option<[**SupportTicketPriorityCreateDto**](SupportTicketPriorityCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_ticket_priority_async

> models::EmptyEnvelope delete_support_ticket_priority_async(tenant_id, support_ticket_priority_id, api_version, x_api_version)
Delete a support ticket priority

Deletes a support ticket priority by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_priority_id** | **uuid::Uuid** |  | [required] |
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


## get_support_ticket_priorities_async

> models::SupportTicketPriorityDtoListEnvelope get_support_ticket_priorities_async(tenant_id, api_version, x_api_version)
Retrieve a list of support ticket priorities

Retrieves a list of support ticket priorities for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketPriorityDtoListEnvelope**](SupportTicketPriorityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_priorities_count_async

> models::Int32Envelope get_support_ticket_priorities_count_async(tenant_id, api_version, x_api_version)
Get the count of support ticket priorities

Returns the total count of support ticket priorities for the specified tenant with OData query support.

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


## get_support_ticket_priority_async

> models::SupportTicketPriorityDtoEnvelope get_support_ticket_priority_async(tenant_id, support_ticket_priority_id, api_version, x_api_version)
Retrieve a support ticket priority by ID

Retrieves a single support ticket priority by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_priority_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketPriorityDtoEnvelope**](SupportTicketPriorityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_support_ticket_priority_async

> models::EmptyEnvelope update_support_ticket_priority_async(tenant_id, support_ticket_priority_id, api_version, x_api_version, support_ticket_priority_update_dto)
Update a support ticket priority

Updates an existing support ticket priority by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_priority_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_priority_update_dto** | Option<[**SupportTicketPriorityUpdateDto**](SupportTicketPriorityUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

