# \ProofsOfDeliveryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#add_proof_of_delivery_line_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines | Add a line to proof of delivery
[**attach_delivery_note_async**](ProofsOfDeliveryApi.md#attach_delivery_note_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/{noteId} | Attach a delivery note
[**create_proof_of_delivery_async**](ProofsOfDeliveryApi.md#create_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery | Create a proof of delivery
[**delete_proof_of_delivery_async**](ProofsOfDeliveryApi.md#delete_proof_of_delivery_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Delete a proof of delivery
[**detach_delivery_note_async**](ProofsOfDeliveryApi.md#detach_delivery_note_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/{noteId} | Detach a delivery note
[**dispute_proof_of_delivery_async**](ProofsOfDeliveryApi.md#dispute_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Dispute | Dispute a proof of delivery
[**get_proof_of_delivery_by_id_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_by_id_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Get proof of delivery by ID
[**get_proof_of_delivery_delivery_notes_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_delivery_notes_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes | Get attached delivery notes
[**get_proof_of_delivery_delivery_notes_count_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_delivery_notes_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/DeliveryNotes/Count | Get delivery notes count
[**get_proof_of_delivery_lines_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_lines_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines | Get proof of delivery lines
[**get_proof_of_delivery_lines_count_async**](ProofsOfDeliveryApi.md#get_proof_of_delivery_lines_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/Count | Get proof of delivery lines count
[**get_proofs_of_delivery_async**](ProofsOfDeliveryApi.md#get_proofs_of_delivery_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery | Get all proofs of delivery
[**get_proofs_of_delivery_count_async**](ProofsOfDeliveryApi.md#get_proofs_of_delivery_count_async) | **GET** /api/v2/LogisticsService/ProofsOfDelivery/Count | Get proofs of delivery count
[**reject_proof_of_delivery_async**](ProofsOfDeliveryApi.md#reject_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Reject | Reject a proof of delivery
[**remove_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#remove_proof_of_delivery_line_async) | **DELETE** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/{lineId} | Remove a proof of delivery line
[**sign_proof_of_delivery_async**](ProofsOfDeliveryApi.md#sign_proof_of_delivery_async) | **POST** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Sign | Sign a proof of delivery
[**update_proof_of_delivery_async**](ProofsOfDeliveryApi.md#update_proof_of_delivery_async) | **PUT** /api/v2/LogisticsService/ProofsOfDelivery/{podId} | Update a proof of delivery
[**update_proof_of_delivery_line_async**](ProofsOfDeliveryApi.md#update_proof_of_delivery_line_async) | **PUT** /api/v2/LogisticsService/ProofsOfDelivery/{podId}/Lines/{lineId} | Update a proof of delivery line



## add_proof_of_delivery_line_async

> models::EmptyEnvelope add_proof_of_delivery_line_async(tenant_id, pod_id, api_version, x_api_version, proof_of_delivery_line_create_dto)
Add a line to proof of delivery

Adds a new line to a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**proof_of_delivery_line_create_dto** | Option<[**ProofOfDeliveryLineCreateDto**](ProofOfDeliveryLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## attach_delivery_note_async

> models::EmptyEnvelope attach_delivery_note_async(tenant_id, pod_id, note_id, api_version, x_api_version)
Attach a delivery note

Attaches a delivery note to a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**note_id** | **uuid::Uuid** |  | [required] |
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


## create_proof_of_delivery_async

> models::EmptyEnvelope create_proof_of_delivery_async(tenant_id, api_version, x_api_version, proof_of_delivery_create_dto)
Create a proof of delivery

Creates a new proof of delivery for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**proof_of_delivery_create_dto** | Option<[**ProofOfDeliveryCreateDto**](ProofOfDeliveryCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_proof_of_delivery_async

> models::EmptyEnvelope delete_proof_of_delivery_async(tenant_id, pod_id, api_version, x_api_version)
Delete a proof of delivery

Deletes a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
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


## detach_delivery_note_async

> models::EmptyEnvelope detach_delivery_note_async(tenant_id, pod_id, note_id, api_version, x_api_version)
Detach a delivery note

Detaches a delivery note from a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**note_id** | **uuid::Uuid** |  | [required] |
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


## dispute_proof_of_delivery_async

> models::EmptyEnvelope dispute_proof_of_delivery_async(tenant_id, pod_id, api_version, x_api_version, dispute_proof_of_delivery_request)
Dispute a proof of delivery

Disputes a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**dispute_proof_of_delivery_request** | Option<[**DisputeProofOfDeliveryRequest**](DisputeProofOfDeliveryRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_proof_of_delivery_by_id_async

> models::ProofOfDeliveryDtoEnvelope get_proof_of_delivery_by_id_async(tenant_id, pod_id, api_version, x_api_version)
Get proof of delivery by ID

Retrieves a specific proof of delivery by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProofOfDeliveryDtoEnvelope**](ProofOfDeliveryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_proof_of_delivery_delivery_notes_async

> models::DeliveryNoteDtoListEnvelope get_proof_of_delivery_delivery_notes_async(tenant_id, pod_id, api_version, x_api_version)
Get attached delivery notes

Retrieves all delivery notes attached to a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
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


## get_proof_of_delivery_delivery_notes_count_async

> models::Int32Envelope get_proof_of_delivery_delivery_notes_count_async(tenant_id, pod_id, api_version, x_api_version)
Get delivery notes count

Returns the count of delivery notes attached to a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
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


## get_proof_of_delivery_lines_async

> models::ProofOfDeliveryLineDtoListEnvelope get_proof_of_delivery_lines_async(tenant_id, pod_id, api_version, x_api_version)
Get proof of delivery lines

Retrieves all lines for a specific proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProofOfDeliveryLineDtoListEnvelope**](ProofOfDeliveryLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_proof_of_delivery_lines_count_async

> models::Int32Envelope get_proof_of_delivery_lines_count_async(tenant_id, pod_id, api_version, x_api_version)
Get proof of delivery lines count

Returns the count of lines for a specific proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
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


## get_proofs_of_delivery_async

> models::ProofOfDeliveryDtoListEnvelope get_proofs_of_delivery_async(tenant_id, api_version, x_api_version)
Get all proofs of delivery

Retrieves all proofs of delivery for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ProofOfDeliveryDtoListEnvelope**](ProofOfDeliveryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_proofs_of_delivery_count_async

> models::Int32Envelope get_proofs_of_delivery_count_async(tenant_id, api_version, x_api_version)
Get proofs of delivery count

Returns the count of proofs of delivery for the specified tenant.

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


## reject_proof_of_delivery_async

> models::EmptyEnvelope reject_proof_of_delivery_async(tenant_id, pod_id, api_version, x_api_version, reject_proof_of_delivery_request)
Reject a proof of delivery

Rejects a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**reject_proof_of_delivery_request** | Option<[**RejectProofOfDeliveryRequest**](RejectProofOfDeliveryRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_proof_of_delivery_line_async

> models::EmptyEnvelope remove_proof_of_delivery_line_async(tenant_id, pod_id, line_id, api_version, x_api_version)
Remove a proof of delivery line

Removes a line from a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
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


## sign_proof_of_delivery_async

> models::EmptyEnvelope sign_proof_of_delivery_async(tenant_id, pod_id, api_version, x_api_version, sign_proof_of_delivery_request)
Sign a proof of delivery

Signs a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**sign_proof_of_delivery_request** | Option<[**SignProofOfDeliveryRequest**](SignProofOfDeliveryRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_proof_of_delivery_async

> models::EmptyEnvelope update_proof_of_delivery_async(tenant_id, pod_id, api_version, x_api_version, proof_of_delivery_update_dto)
Update a proof of delivery

Updates an existing proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**proof_of_delivery_update_dto** | Option<[**ProofOfDeliveryUpdateDto**](ProofOfDeliveryUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_proof_of_delivery_line_async

> models::EmptyEnvelope update_proof_of_delivery_line_async(tenant_id, pod_id, line_id, api_version, x_api_version, proof_of_delivery_line_update_dto)
Update a proof of delivery line

Updates an existing line on a proof of delivery.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pod_id** | **uuid::Uuid** |  | [required] |
**line_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**proof_of_delivery_line_update_dto** | Option<[**ProofOfDeliveryLineUpdateDto**](ProofOfDeliveryLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

