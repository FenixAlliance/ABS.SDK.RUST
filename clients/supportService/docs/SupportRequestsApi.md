# \SupportRequestsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_support_request_async**](SupportRequestsApi.md#create_support_request_async) | **POST** /api/v2/SupportService/SupportRequests | Create a new support request
[**delete_support_request_async**](SupportRequestsApi.md#delete_support_request_async) | **DELETE** /api/v2/SupportService/SupportRequests/{supportRequestId} | Delete a support request
[**get_support_request_async**](SupportRequestsApi.md#get_support_request_async) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId} | Retrieve a support request by ID
[**get_support_request_attachment_by_request**](SupportRequestsApi.md#get_support_request_attachment_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments/{attachmentId} | Retrieve a specific attachment for a support request
[**get_support_request_attachments_by_request**](SupportRequestsApi.md#get_support_request_attachments_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments | Retrieve attachments for a support request
[**get_support_request_attachments_count_by_request**](SupportRequestsApi.md#get_support_request_attachments_count_by_request) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments/Count | Get the count of attachments for a support request
[**get_support_request_tickets_async**](SupportRequestsApi.md#get_support_request_tickets_async) | **GET** /api/v2/SupportService/SupportRequests/{supportRequestId}/Tickets | Retrieve tickets for a support request
[**get_support_requests_async**](SupportRequestsApi.md#get_support_requests_async) | **GET** /api/v2/SupportService/SupportRequests | Retrieve a list of support requests
[**get_support_requests_count_async**](SupportRequestsApi.md#get_support_requests_count_async) | **GET** /api/v2/SupportService/SupportRequests/Count | Get the count of support requests
[**relate_support_request_to_attachment_async**](SupportRequestsApi.md#relate_support_request_to_attachment_async) | **POST** /api/v2/SupportService/SupportRequests/{supportRequestId}/Attachments | Add an attachment to a support request
[**update_support_request_async**](SupportRequestsApi.md#update_support_request_async) | **PUT** /api/v2/SupportService/SupportRequests/{supportRequestId} | Update a support request



## create_support_request_async

> models::EmptyEnvelope create_support_request_async(tenant_id, api_version, x_api_version, support_request_create_dto)
Create a new support request

Creates a new support request for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_request_create_dto** | Option<[**SupportRequestCreateDto**](SupportRequestCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_support_request_async

> models::EmptyEnvelope delete_support_request_async(tenant_id, support_request_id, api_version, x_api_version)
Delete a support request

Deletes a support request by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
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


## get_support_request_async

> models::SupportRequestDtoEnvelope get_support_request_async(tenant_id, support_request_id, api_version, x_api_version)
Retrieve a support request by ID

Retrieves a single support request by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestDtoEnvelope**](SupportRequestDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_request_attachment_by_request

> models::SupportRequestAttachmentDtoEnvelope get_support_request_attachment_by_request(tenant_id, support_request_id, attachment_id, api_version, x_api_version)
Retrieve a specific attachment for a support request

Retrieves a single attachment by its ID for a specific support request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
**attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestAttachmentDtoEnvelope**](SupportRequestAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_request_attachments_by_request

> models::SupportRequestAttachmentDtoListEnvelope get_support_request_attachments_by_request(tenant_id, support_request_id, api_version, x_api_version)
Retrieve attachments for a support request

Retrieves the list of attachments associated with a specific support request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestAttachmentDtoListEnvelope**](SupportRequestAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_request_attachments_count_by_request

> models::Int32Envelope get_support_request_attachments_count_by_request(tenant_id, support_request_id, api_version, x_api_version)
Get the count of attachments for a support request

Returns the total count of attachments for a specific support request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
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


## get_support_request_tickets_async

> models::SupportTicketDtoListEnvelope get_support_request_tickets_async(tenant_id, support_request_id, api_version, x_api_version)
Retrieve tickets for a support request

Retrieves the list of support tickets associated with a specific support request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
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


## get_support_requests_async

> models::SupportRequestDtoListEnvelope get_support_requests_async(tenant_id, api_version, x_api_version)
Retrieve a list of support requests

Retrieves a list of support requests for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SupportRequestDtoListEnvelope**](SupportRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_support_requests_count_async

> models::Int32Envelope get_support_requests_count_async(tenant_id, api_version, x_api_version)
Get the count of support requests

Returns the total count of support requests for the specified tenant with OData query support.

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


## relate_support_request_to_attachment_async

> models::EmptyEnvelope relate_support_request_to_attachment_async(tenant_id, support_request_id, api_version, x_api_version, support_request_attachment_create_dto)
Add an attachment to a support request

Creates a new attachment and associates it with the specified support request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_request_attachment_create_dto** | Option<[**SupportRequestAttachmentCreateDto**](SupportRequestAttachmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_support_request_async

> models::EmptyEnvelope update_support_request_async(tenant_id, support_request_id, api_version, x_api_version, support_request_update_dto)
Update a support request

Updates an existing support request by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**support_request_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**support_request_update_dto** | Option<[**SupportRequestUpdateDto**](SupportRequestUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

