# \PriceListsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_price_list_async**](PriceListsApi.md#create_price_list_async) | **POST** /api/v2/PricingService/PriceLists | Creates a new price list
[**create_price_list_prices_async**](PriceListsApi.md#create_price_list_prices_async) | **POST** /api/v2/PricingService/PriceLists/{priceListId}/Prices | Creates a price list entry
[**delete_price_list_async**](PriceListsApi.md#delete_price_list_async) | **DELETE** /api/v2/PricingService/PriceLists/{priceListId} | Deletes a price list
[**delete_price_list_price_async**](PriceListsApi.md#delete_price_list_price_async) | **DELETE** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Deletes a price list entry
[**get_price_list_async**](PriceListsApi.md#get_price_list_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId} | Gets a price list by ID
[**get_price_list_price_async**](PriceListsApi.md#get_price_list_price_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Gets a price list entry by ID
[**get_price_list_prices_async**](PriceListsApi.md#get_price_list_prices_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId}/Prices | Retrieves prices in a price list
[**get_price_lists_async**](PriceListsApi.md#get_price_lists_async) | **GET** /api/v2/PricingService/PriceLists | Retrieves all price lists
[**get_price_lists_count_async**](PriceListsApi.md#get_price_lists_count_async) | **GET** /api/v2/PricingService/PriceLists/Count | Counts price lists
[**update_price_list_async**](PriceListsApi.md#update_price_list_async) | **PUT** /api/v2/PricingService/PriceLists/{priceListId} | Updates a price list
[**update_price_list_price_async**](PriceListsApi.md#update_price_list_price_async) | **PUT** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Updates a price list entry



## create_price_list_async

> models::EmptyEnvelope create_price_list_async(tenant_id, price_list_create_dto)
Creates a new price list

Creates a new price list for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_create_dto** | Option<[**PriceListCreateDto**](PriceListCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_price_list_prices_async

> models::EmptyEnvelope create_price_list_prices_async(tenant_id, price_list_id, item_price_create_dto)
Creates a price list entry

Creates a new price entry in the specified price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**item_price_create_dto** | Option<[**ItemPriceCreateDto**](ItemPriceCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_price_list_async

> models::EmptyEnvelope delete_price_list_async(tenant_id, price_list_id)
Deletes a price list

Deletes the specified price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_price_list_price_async

> models::EmptyEnvelope delete_price_list_price_async(tenant_id, price_list_id, price_id)
Deletes a price list entry

Deletes the specified price entry from a price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**price_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_list_async

> models::PriceListDtoEnvelope get_price_list_async(tenant_id, price_list_id)
Gets a price list by ID

Retrieves the details of a price list using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PriceListDtoEnvelope**](PriceListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_list_price_async

> models::ItemPriceDtoEnvelope get_price_list_price_async(tenant_id, price_list_id, price_id)
Gets a price list entry by ID

Retrieves a specific price entry from a price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**price_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ItemPriceDtoEnvelope**](ItemPriceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_list_prices_async

> models::ItemPriceDtoListEnvelope get_price_list_prices_async(tenant_id, price_list_id, item_id)
Retrieves prices in a price list

Gets all price entries for a specific price list with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::ItemPriceDtoListEnvelope**](ItemPriceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_lists_async

> models::PriceListDtoListEnvelope get_price_lists_async(tenant_id)
Retrieves all price lists

Gets all price lists for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PriceListDtoListEnvelope**](PriceListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_price_lists_count_async

> models::Int32Envelope get_price_lists_count_async(tenant_id)
Counts price lists

Gets the count of price lists for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_price_list_async

> models::EmptyEnvelope update_price_list_async(tenant_id, price_list_id, price_list_update_dto)
Updates a price list

Updates the specified price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**price_list_update_dto** | Option<[**PriceListUpdateDto**](PriceListUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_price_list_price_async

> models::EmptyEnvelope update_price_list_price_async(tenant_id, price_list_id, price_id, item_price_update_dto)
Updates a price list entry

Updates the specified price entry in a price list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**price_list_id** | **uuid::Uuid** |  | [required] |
**price_id** | **uuid::Uuid** |  | [required] |
**item_price_update_dto** | Option<[**ItemPriceUpdateDto**](ItemPriceUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

