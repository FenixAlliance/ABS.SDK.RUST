# \ItemAttributeOptionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_attribute_option_async**](ItemAttributeOptionsApi.md#create_item_attribute_option_async) | **POST** /api/v2/CatalogService/ItemAttributeOptions | Create a new item attribute option
[**delete_item_attribute_option_async**](ItemAttributeOptionsApi.md#delete_item_attribute_option_async) | **DELETE** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Delete an item attribute option
[**get_item_attribute_option_by_id_async**](ItemAttributeOptionsApi.md#get_item_attribute_option_by_id_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Get item attribute option by ID
[**get_item_attribute_options_async**](ItemAttributeOptionsApi.md#get_item_attribute_options_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions | Get all item attribute options
[**get_item_attribute_options_count_async**](ItemAttributeOptionsApi.md#get_item_attribute_options_count_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions/Count | Get item attribute options count
[**update_item_attribute_option_async**](ItemAttributeOptionsApi.md#update_item_attribute_option_async) | **PUT** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Update an item attribute option



## create_item_attribute_option_async

> models::ItemAttributeOptionDtoEnvelope create_item_attribute_option_async(tenant_id, api_version, x_api_version, item_attribute_option_create_dto)
Create a new item attribute option

Creates a new item attribute option for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attribute_option_create_dto** | Option<[**ItemAttributeOptionCreateDto**](ItemAttributeOptionCreateDto.md)> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_attribute_option_async

> delete_item_attribute_option_async(tenant_id, item_attribute_option_id, api_version, x_api_version)
Delete an item attribute option

Deletes an item attribute option for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
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


## get_item_attribute_option_by_id_async

> models::ItemAttributeOptionDtoEnvelope get_item_attribute_option_by_id_async(item_attribute_option_id, tenant_id, api_version, x_api_version)
Get item attribute option by ID

Retrieves a specific item attribute option by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_attribute_options_async

> models::ItemAttributeOptionDtoListEnvelope get_item_attribute_options_async(tenant_id, api_version, x_api_version)
Get all item attribute options

Retrieves all item attribute options for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoListEnvelope**](ItemAttributeOptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_attribute_options_count_async

> models::Int32Envelope get_item_attribute_options_count_async(tenant_id, api_version, x_api_version)
Get item attribute options count

Returns the count of item attribute options for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## update_item_attribute_option_async

> models::ItemAttributeOptionDtoEnvelope update_item_attribute_option_async(tenant_id, item_attribute_option_id, api_version, x_api_version, item_attribute_option_update_dto)
Update an item attribute option

Updates an existing item attribute option for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attribute_option_update_dto** | Option<[**ItemAttributeOptionUpdateDto**](ItemAttributeOptionUpdateDto.md)> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

