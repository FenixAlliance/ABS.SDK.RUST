# \ContactRelationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_relation_async**](ContactRelationsApi.md#create_contact_relation_async) | **POST** /api/v2/CrmService/ContactRelations | Create a new contact relation
[**delete_contact_relation_async**](ContactRelationsApi.md#delete_contact_relation_async) | **DELETE** /api/v2/CrmService/ContactRelations/{id} | Delete a contact relation
[**get_contact_relation_by_id_async**](ContactRelationsApi.md#get_contact_relation_by_id_async) | **GET** /api/v2/CrmService/ContactRelations/{id} | Get contact relation by ID
[**get_contact_relations_async**](ContactRelationsApi.md#get_contact_relations_async) | **GET** /api/v2/CrmService/ContactRelations | Get all contact relations
[**get_contact_relations_count_async**](ContactRelationsApi.md#get_contact_relations_count_async) | **GET** /api/v2/CrmService/ContactRelations/Count | Get contact relations count
[**patch_contact_relation_async**](ContactRelationsApi.md#patch_contact_relation_async) | **PATCH** /api/v2/CrmService/ContactRelations/{id} | Patch a contact relation
[**update_contact_relation_async**](ContactRelationsApi.md#update_contact_relation_async) | **PUT** /api/v2/CrmService/ContactRelations/{id} | Update a contact relation



## create_contact_relation_async

> create_contact_relation_async(tenant_id, api_version, x_api_version, contact_relation_create_dto)
Create a new contact relation

Creates a new contact relation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_create_dto** | Option<[**ContactRelationCreateDto**](ContactRelationCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_relation_async

> delete_contact_relation_async(tenant_id, id, api_version, x_api_version)
Delete a contact relation

Deletes a contact relation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_relation_by_id_async

> models::ContactRelationDto get_contact_relation_by_id_async(tenant_id, id, api_version, x_api_version)
Get contact relation by ID

Retrieves a specific contact relation by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactRelationDto**](ContactRelationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_relations_async

> models::ContactRelationDtoListEnvelope get_contact_relations_async(tenant_id, api_version, x_api_version, contact_relation_dto_collection_query_parameters)
Get all contact relations

Retrieves all contact relations for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_dto_collection_query_parameters** | Option<[**ContactRelationDtoCollectionQueryParameters**](ContactRelationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ContactRelationDtoListEnvelope**](ContactRelationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_relations_count_async

> models::Int32Envelope get_contact_relations_count_async(tenant_id, api_version, x_api_version, contact_relation_dto_collection_query_parameters)
Get contact relations count

Returns the count of contact relations for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_dto_collection_query_parameters** | Option<[**ContactRelationDtoCollectionQueryParameters**](ContactRelationDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_contact_relation_async

> models::EmptyEnvelope patch_contact_relation_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a contact relation

Patch a contact relation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_contact_relation_async

> update_contact_relation_async(tenant_id, id, api_version, x_api_version, contact_relation_update_dto)
Update a contact relation

Updates an existing contact relation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_update_dto** | Option<[**ContactRelationUpdateDto**](ContactRelationUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

