# \ContactRelationTypesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_relation_type_async**](ContactRelationTypesApi.md#create_contact_relation_type_async) | **POST** /api/v2/CrmService/ContactRelationTypes | Create a new contact relation type
[**delete_contact_relation_type_async**](ContactRelationTypesApi.md#delete_contact_relation_type_async) | **DELETE** /api/v2/CrmService/ContactRelationTypes/{id} | Delete a contact relation type
[**get_contact_relation_type_by_id_async**](ContactRelationTypesApi.md#get_contact_relation_type_by_id_async) | **GET** /api/v2/CrmService/ContactRelationTypes/{id} | Get contact relation type by ID
[**get_contact_relation_types_async**](ContactRelationTypesApi.md#get_contact_relation_types_async) | **GET** /api/v2/CrmService/ContactRelationTypes | Get all contact relation types
[**get_contact_relation_types_count_async**](ContactRelationTypesApi.md#get_contact_relation_types_count_async) | **GET** /api/v2/CrmService/ContactRelationTypes/Count | Get contact relation types count
[**patch_contact_relation_type_async**](ContactRelationTypesApi.md#patch_contact_relation_type_async) | **PATCH** /api/v2/CrmService/ContactRelationTypes/{id} | Patch a contact relation type
[**update_contact_relation_type_async**](ContactRelationTypesApi.md#update_contact_relation_type_async) | **PUT** /api/v2/CrmService/ContactRelationTypes/{id} | Update a contact relation type



## create_contact_relation_type_async

> create_contact_relation_type_async(tenant_id, api_version, x_api_version, contact_relation_type_create_dto)
Create a new contact relation type

Creates a new contact relation type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_type_create_dto** | Option<[**ContactRelationTypeCreateDto**](ContactRelationTypeCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_relation_type_async

> delete_contact_relation_type_async(tenant_id, id, api_version, x_api_version)
Delete a contact relation type

Deletes a contact relation type for the specified tenant.

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


## get_contact_relation_type_by_id_async

> models::ContactRelationTypeDto get_contact_relation_type_by_id_async(tenant_id, id, api_version, x_api_version)
Get contact relation type by ID

Retrieves a specific contact relation type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactRelationTypeDto**](ContactRelationTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_relation_types_async

> models::ContactRelationTypeDtoListEnvelope get_contact_relation_types_async(tenant_id, api_version, x_api_version)
Get all contact relation types

Retrieves all contact relation types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactRelationTypeDtoListEnvelope**](ContactRelationTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_relation_types_count_async

> models::Int32Envelope get_contact_relation_types_count_async(tenant_id, api_version, x_api_version)
Get contact relation types count

Returns the count of contact relation types for the specified tenant.

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


## patch_contact_relation_type_async

> models::EmptyEnvelope patch_contact_relation_type_async(tenant_id, id, api_version, x_api_version, operation)
Patch a contact relation type

Patch a contact relation type

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## update_contact_relation_type_async

> update_contact_relation_type_async(tenant_id, id, api_version, x_api_version, contact_relation_type_update_dto)
Update a contact relation type

Updates an existing contact relation type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_relation_type_update_dto** | Option<[**ContactRelationTypeUpdateDto**](ContactRelationTypeUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

