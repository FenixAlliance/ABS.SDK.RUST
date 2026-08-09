# \ContactSourcesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_source_async**](ContactSourcesApi.md#create_contact_source_async) | **POST** /api/v2/CrmService/ContactSources | Create a new contact source
[**delete_contact_source_async**](ContactSourcesApi.md#delete_contact_source_async) | **DELETE** /api/v2/CrmService/ContactSources/{id} | Delete a contact source
[**get_contact_source_by_id_async**](ContactSourcesApi.md#get_contact_source_by_id_async) | **GET** /api/v2/CrmService/ContactSources/{id} | Get contact source by ID
[**get_contact_sources_async**](ContactSourcesApi.md#get_contact_sources_async) | **GET** /api/v2/CrmService/ContactSources | Get all contact sources
[**get_contact_sources_count_async**](ContactSourcesApi.md#get_contact_sources_count_async) | **GET** /api/v2/CrmService/ContactSources/Count | Get contact sources count
[**patch_contact_source_async**](ContactSourcesApi.md#patch_contact_source_async) | **PATCH** /api/v2/CrmService/ContactSources/{id} | Patch a contact source
[**update_contact_source_async**](ContactSourcesApi.md#update_contact_source_async) | **PUT** /api/v2/CrmService/ContactSources/{id} | Update a contact source



## create_contact_source_async

> create_contact_source_async(tenant_id, api_version, x_api_version, contact_source_create_dto)
Create a new contact source

Creates a new contact source for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_source_create_dto** | Option<[**ContactSourceCreateDto**](ContactSourceCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_source_async

> delete_contact_source_async(tenant_id, id, api_version, x_api_version)
Delete a contact source

Deletes a contact source for the specified tenant.

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


## get_contact_source_by_id_async

> models::ContactSourceDto get_contact_source_by_id_async(tenant_id, id, api_version, x_api_version)
Get contact source by ID

Retrieves a specific contact source by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactSourceDto**](ContactSourceDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_sources_async

> models::ContactSourceDtoListEnvelope get_contact_sources_async(tenant_id, api_version, x_api_version, contact_source_dto_collection_query_parameters)
Get all contact sources

Retrieves all contact sources for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_source_dto_collection_query_parameters** | Option<[**ContactSourceDtoCollectionQueryParameters**](ContactSourceDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ContactSourceDtoListEnvelope**](ContactSourceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_sources_count_async

> models::Int32Envelope get_contact_sources_count_async(tenant_id, api_version, x_api_version, contact_source_dto_collection_query_parameters)
Get contact sources count

Returns the count of contact sources for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_source_dto_collection_query_parameters** | Option<[**ContactSourceDtoCollectionQueryParameters**](ContactSourceDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_contact_source_async

> models::EmptyEnvelope patch_contact_source_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a contact source

Patch a contact source

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


## update_contact_source_async

> update_contact_source_async(tenant_id, id, api_version, x_api_version, contact_source_update_dto)
Update a contact source

Updates an existing contact source for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_source_update_dto** | Option<[**ContactSourceUpdateDto**](ContactSourceUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

