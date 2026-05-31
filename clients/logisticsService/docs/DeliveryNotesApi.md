# \DeliveryNotesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_note_async**](DeliveryNotesApi.md#create_delivery_note_async) | **POST** /api/v2/LogisticsService/DeliveryNotes | Create a delivery note
[**delete_delivery_note_async**](DeliveryNotesApi.md#delete_delivery_note_async) | **DELETE** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Delete a delivery note
[**get_delivery_note_by_id_async**](DeliveryNotesApi.md#get_delivery_note_by_id_async) | **GET** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Get delivery note by ID
[**get_delivery_notes_async**](DeliveryNotesApi.md#get_delivery_notes_async) | **GET** /api/v2/LogisticsService/DeliveryNotes | Get all delivery notes
[**get_delivery_notes_count_async**](DeliveryNotesApi.md#get_delivery_notes_count_async) | **GET** /api/v2/LogisticsService/DeliveryNotes/Count | Get delivery notes count
[**update_delivery_note_async**](DeliveryNotesApi.md#update_delivery_note_async) | **PUT** /api/v2/LogisticsService/DeliveryNotes/{deliveryNoteId} | Update a delivery note



## create_delivery_note_async

> models::EmptyEnvelope create_delivery_note_async(tenant_id, api_version, x_api_version, delivery_note_create_dto)
Create a delivery note

Creates a new delivery note.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**delivery_note_create_dto** | Option<[**DeliveryNoteCreateDto**](DeliveryNoteCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_delivery_note_async

> models::EmptyEnvelope delete_delivery_note_async(tenant_id, delivery_note_id, api_version, x_api_version)
Delete a delivery note

Deletes a delivery note.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**delivery_note_id** | **uuid::Uuid** |  | [required] |
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


## get_delivery_note_by_id_async

> models::DeliveryNoteDtoEnvelope get_delivery_note_by_id_async(tenant_id, delivery_note_id, api_version, x_api_version)
Get delivery note by ID

Retrieves a specific delivery note.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**delivery_note_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::DeliveryNoteDtoEnvelope**](DeliveryNoteDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_delivery_notes_async

> models::DeliveryNoteDtoListEnvelope get_delivery_notes_async(tenant_id, api_version, x_api_version)
Get all delivery notes

Retrieves all delivery notes for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::DeliveryNoteDtoListEnvelope**](DeliveryNoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_delivery_notes_count_async

> models::Int32Envelope get_delivery_notes_count_async(tenant_id, api_version, x_api_version)
Get delivery notes count

Returns the count of delivery notes.

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


## update_delivery_note_async

> models::EmptyEnvelope update_delivery_note_async(tenant_id, delivery_note_id, api_version, x_api_version, delivery_note_update_dto)
Update a delivery note

Updates an existing delivery note.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**delivery_note_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**delivery_note_update_dto** | Option<[**DeliveryNoteUpdateDto**](DeliveryNoteUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

