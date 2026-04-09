# \MarketingListsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_marketing_list_async**](MarketingListsApi.md#create_marketing_list_async) | **POST** /api/v2/MarketingService/MarketingLists | Create a marketing list
[**delete_marketing_list_async**](MarketingListsApi.md#delete_marketing_list_async) | **DELETE** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Delete a marketing list
[**get_marketing_list_details_async**](MarketingListsApi.md#get_marketing_list_details_async) | **GET** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Get marketing list by ID
[**get_marketing_list_o_data_async**](MarketingListsApi.md#get_marketing_list_o_data_async) | **GET** /api/v2/MarketingService/MarketingLists | Get marketing lists
[**get_marketing_lists_count_async**](MarketingListsApi.md#get_marketing_lists_count_async) | **GET** /api/v2/MarketingService/MarketingLists/Count | Get marketing lists count
[**update_marketing_list_async**](MarketingListsApi.md#update_marketing_list_async) | **PUT** /api/v2/MarketingService/MarketingLists/{marketinglistId} | Update a marketing list



## create_marketing_list_async

> models::EmptyEnvelope create_marketing_list_async(tenant_id, marketing_list_create_dto, api_version, x_api_version)
Create a marketing list

Creates a new marketing list for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_list_create_dto** | [**MarketingListCreateDto**](MarketingListCreateDto.md) |  | [required] |
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


## delete_marketing_list_async

> models::EmptyEnvelope delete_marketing_list_async(tenant_id, marketinglist_id, api_version, x_api_version)
Delete a marketing list

Deletes a marketing list by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketinglist_id** | **uuid::Uuid** |  | [required] |
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


## get_marketing_list_details_async

> models::MarketingListDtoEnvelope get_marketing_list_details_async(tenant_id, marketinglist_id, api_version, x_api_version)
Get marketing list by ID

Retrieves the details of a specific marketing list by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketinglist_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingListDtoEnvelope**](MarketingListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_list_o_data_async

> models::MarketingListDtoListEnvelope get_marketing_list_o_data_async(tenant_id, api_version, x_api_version)
Get marketing lists

Retrieves a collection of marketing lists for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingListDtoListEnvelope**](MarketingListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_lists_count_async

> models::Int32Envelope get_marketing_lists_count_async(tenant_id, api_version, x_api_version)
Get marketing lists count

Returns the count of marketing lists for the specified tenant using OData query options.

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


## update_marketing_list_async

> models::EmptyEnvelope update_marketing_list_async(tenant_id, marketinglist_id, marketing_list_update_dto, api_version, x_api_version)
Update a marketing list

Updates an existing marketing list by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketinglist_id** | **uuid::Uuid** |  | [required] |
**marketing_list_update_dto** | [**MarketingListUpdateDto**](MarketingListUpdateDto.md) |  | [required] |
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

