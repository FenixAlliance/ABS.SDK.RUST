# \SupportTicketsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_ticket_async**](SupportTicketsApi.md#create_support_ticket_async) | **POST** /api/v2/SupportService/SupportTickets | Create a new support ticket
[**delete_support_ticket_async**](SupportTicketsApi.md#delete_support_ticket_async) | **DELETE** /api/v2/SupportService/SupportTickets/{supportTicketId} | Delete a support ticket
[**delete_support_ticket_conversation_async**](SupportTicketsApi.md#delete_support_ticket_conversation_async) | **DELETE** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId} | Delete a conversation from a support ticket
[**get_support_ticket_async**](SupportTicketsApi.md#get_support_ticket_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId} | Retrieve a support ticket by ID
[**get_support_ticket_conversation_async**](SupportTicketsApi.md#get_support_ticket_conversation_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId} | Retrieve a specific conversation for a support ticket
[**get_support_ticket_conversation_messages_async**](SupportTicketsApi.md#get_support_ticket_conversation_messages_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations/{supportTicketConversationId}/Messages | Retrieve messages for a support ticket conversation
[**get_support_ticket_conversations_async**](SupportTicketsApi.md#get_support_ticket_conversations_async) | **GET** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations | Retrieve conversations for a support ticket
[**get_support_tickets_async**](SupportTicketsApi.md#get_support_tickets_async) | **GET** /api/v2/SupportService/SupportTickets | Retrieve a list of support tickets
[**get_support_tickets_count_async**](SupportTicketsApi.md#get_support_tickets_count_async) | **GET** /api/v2/SupportService/SupportTickets/Count | Get the count of support tickets
[**relate_support_ticket_to_conversation_async**](SupportTicketsApi.md#relate_support_ticket_to_conversation_async) | **POST** /api/v2/SupportService/SupportTickets/{supportTicketId}/Conversations | Create a conversation for a support ticket
[**update_support_ticket_async**](SupportTicketsApi.md#update_support_ticket_async) | **PUT** /api/v2/SupportService/SupportTickets/{supportTicketId} | Update a support ticket



## create_support_ticket_async

> models::EmptyEnvelope create_support_ticket_async(tenant_id, api_version, x_api_version, support_ticket_create_dto)
Create a new support ticket

Creates a new support ticket for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_create_dto** | Option<[**SupportTicketCreateDto**](SupportTicketCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_ticket_async

> models::EmptyEnvelope delete_support_ticket_async(tenant_id, support_ticket_id, api_version, x_api_version)
Delete a support ticket

Deletes a support ticket by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
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


## delete_support_ticket_conversation_async

> models::EmptyEnvelope delete_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, api_version, x_api_version)
Delete a conversation from a support ticket

Deletes a specific conversation from a support ticket.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**support_ticket_conversation_id** | **uuid::Uuid** |  | [required] |
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


## get_support_ticket_async

> models::SupportTicketDtoEnvelope get_support_ticket_async(tenant_id, support_ticket_id, api_version, x_api_version)
Retrieve a support ticket by ID

Retrieves a single support ticket by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketDtoEnvelope**](SupportTicketDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_conversation_async

> models::SupportTicketConversationDtoEnvelope get_support_ticket_conversation_async(tenant_id, support_ticket_id, support_ticket_conversation_id, api_version, x_api_version)
Retrieve a specific conversation for a support ticket

Retrieves a single conversation by its ID for a specific support ticket.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**support_ticket_conversation_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketConversationDtoEnvelope**](SupportTicketConversationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_conversation_messages_async

> models::PrivateMessageDtoListEnvelope get_support_ticket_conversation_messages_async(tenant_id, support_ticket_id, support_ticket_conversation_id, page_number, page_size, api_version, x_api_version)
Retrieve messages for a support ticket conversation

Retrieves the list of messages within a specific conversation of a support ticket.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**support_ticket_conversation_id** | **uuid::Uuid** |  | [required] |
**page_number** | Option<**i32**> |  |  |
**page_size** | Option<**i32**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PrivateMessageDtoListEnvelope**](PrivateMessageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_ticket_conversations_async

> models::SupportTicketConversationDtoListEnvelope get_support_ticket_conversations_async(tenant_id, support_ticket_id, api_version, x_api_version)
Retrieve conversations for a support ticket

Retrieves the list of conversations associated with a specific support ticket.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketConversationDtoListEnvelope**](SupportTicketConversationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_tickets_async

> models::SupportTicketDtoListEnvelope get_support_tickets_async(tenant_id, api_version, x_api_version)
Retrieve a list of support tickets

Retrieves a list of support tickets for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportTicketDtoListEnvelope**](SupportTicketDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_tickets_count_async

> models::Int32Envelope get_support_tickets_count_async(tenant_id, api_version, x_api_version)
Get the count of support tickets

Returns the total count of support tickets for the specified tenant with OData query support.

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


## relate_support_ticket_to_conversation_async

> models::EmptyEnvelope relate_support_ticket_to_conversation_async(tenant_id, support_ticket_id, api_version, x_api_version, support_ticket_conversation_create_dto)
Create a conversation for a support ticket

Creates a new conversation and associates it with the specified support ticket.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_conversation_create_dto** | Option<[**SupportTicketConversationCreateDto**](SupportTicketConversationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_support_ticket_async

> models::EmptyEnvelope update_support_ticket_async(tenant_id, support_ticket_id, api_version, x_api_version, support_ticket_update_dto)
Update a support ticket

Updates an existing support ticket by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_ticket_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_ticket_update_dto** | Option<[**SupportTicketUpdateDto**](SupportTicketUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

