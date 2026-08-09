# \BusinessRelationshipsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_business_relationship_async**](BusinessRelationshipsApi.md#create_business_relationship_async) | **POST** /api/v2/TenantsService/BusinessRelationships | Create a business relationship
[**delete_business_relationship_async**](BusinessRelationshipsApi.md#delete_business_relationship_async) | **DELETE** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Delete a business relationship
[**get_business_relationship_by_id_async**](BusinessRelationshipsApi.md#get_business_relationship_by_id_async) | **GET** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Get business relationship by ID
[**get_business_relationships_async**](BusinessRelationshipsApi.md#get_business_relationships_async) | **GET** /api/v2/TenantsService/BusinessRelationships | Get business relationships
[**get_business_relationships_count_async**](BusinessRelationshipsApi.md#get_business_relationships_count_async) | **GET** /api/v2/TenantsService/BusinessRelationships/Count | Get business relationships count
[**update_business_relationship_async**](BusinessRelationshipsApi.md#update_business_relationship_async) | **PUT** /api/v2/TenantsService/BusinessRelationships/{businessRelationshipId} | Update a business relationship



## create_business_relationship_async

> models::EmptyEnvelope create_business_relationship_async(tenant_id, business_relationship_create_dto, api_version, x_api_version)
Create a business relationship

Creates a new business relationship owned by the specified parent tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_relationship_create_dto** | [**BusinessRelationshipCreateDto**](BusinessRelationshipCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_business_relationship_async

> models::EmptyEnvelope delete_business_relationship_async(tenant_id, business_relationship_id, api_version, x_api_version)
Delete a business relationship

Deletes a business relationship by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_relationship_id** | **uuid::Uuid** |  | [required] |
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


## get_business_relationship_by_id_async

> models::BusinessRelationshipDtoEnvelope get_business_relationship_by_id_async(tenant_id, business_relationship_id, api_version, x_api_version)
Get business relationship by ID

Retrieves the details of a specific business relationship by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_relationship_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessRelationshipDtoEnvelope**](BusinessRelationshipDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_relationships_async

> models::BusinessRelationshipDtoListEnvelope get_business_relationships_async(tenant_id, api_version, x_api_version, business_relationship_dto_collection_query_parameters)
Get business relationships

Retrieves the child business relationships owned by the specified parent tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**business_relationship_dto_collection_query_parameters** | Option<[**BusinessRelationshipDtoCollectionQueryParameters**](BusinessRelationshipDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::BusinessRelationshipDtoListEnvelope**](BusinessRelationshipDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_relationships_count_async

> models::Int32Envelope get_business_relationships_count_async(tenant_id, api_version, x_api_version, business_relationship_dto_collection_query_parameters)
Get business relationships count

Returns the count of child business relationships owned by the specified parent tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**business_relationship_dto_collection_query_parameters** | Option<[**BusinessRelationshipDtoCollectionQueryParameters**](BusinessRelationshipDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_business_relationship_async

> models::EmptyEnvelope update_business_relationship_async(tenant_id, business_relationship_id, business_relationship_update_dto, api_version, x_api_version)
Update a business relationship

Updates an existing business relationship by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_relationship_id** | **uuid::Uuid** |  | [required] |
**business_relationship_update_dto** | [**BusinessRelationshipUpdateDto**](BusinessRelationshipUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

