# \CompareApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_item_to_compare_table_async**](CompareApi.md#add_item_to_compare_table_async) | **POST** /api/v2/CartService/Compare | Add an item to the compare table
[**get_item_to_compare_record**](CompareApi.md#get_item_to_compare_record) | **GET** /api/v2/CartService/Compare/{recordId}/Details | Get compare record details
[**get_item_to_compare_records**](CompareApi.md#get_item_to_compare_records) | **GET** /api/v2/CartService/Compare/{cartId} | Get items to compare in a cart
[**remove_item_from_compare_table**](CompareApi.md#remove_item_from_compare_table) | **DELETE** /api/v2/CartService/Compare/{recordId} | Remove an item from the compare table



## add_item_to_compare_table_async

> models::ItemCartRecordDto add_item_to_compare_table_async(api_version, x_api_version, add_product_to_compare_request)
Add an item to the compare table

Adds a product to the compare table for the specified cart with tracking.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**add_product_to_compare_request** | Option<[**AddProductToCompareRequest**](AddProductToCompareRequest.md)> |  |  |

### Return type

[**models::ItemCartRecordDto**](ItemCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_to_compare_record

> models::ItemToCompareCartRecordDtoEnvelope get_item_to_compare_record(record_id, api_version, x_api_version)
Get compare record details

Retrieves the details of a specific item-to-compare cart record.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemToCompareCartRecordDtoEnvelope**](ItemToCompareCartRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_to_compare_records

> models::ItemToCompareCartRecordDtoListEnvelope get_item_to_compare_records(cart_id, api_version, x_api_version)
Get items to compare in a cart

Retrieves all items added to the compare table for the specified cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemToCompareCartRecordDtoListEnvelope**](ItemToCompareCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_item_from_compare_table

> models::ItemToCompareCartRecordDto remove_item_from_compare_table(record_id, api_version, x_api_version)
Remove an item from the compare table

Removes a specific record from the compare table by its record ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemToCompareCartRecordDto**](ItemToCompareCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

