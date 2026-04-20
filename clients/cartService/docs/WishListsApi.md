# \WishListsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_product_to_wish_list**](WishListsApi.md#add_product_to_wish_list) | **POST** /api/v2/CartService/WishLists/Records | Add a product to a wish list
[**create_wish_list**](WishListsApi.md#create_wish_list) | **POST** /api/v2/CartService/WishLists | Create a wish list
[**delete_wish_list**](WishListsApi.md#delete_wish_list) | **DELETE** /api/v2/CartService/WishLists/{wishListId} | Delete a wish list
[**delete_wish_list_record**](WishListsApi.md#delete_wish_list_record) | **DELETE** /api/v2/CartService/WishLists/Records/{recordId} | Delete a wish list record
[**get_cart_wish_list_details_async**](WishListsApi.md#get_cart_wish_list_details_async) | **GET** /api/v2/CartService/WishLists/{wishListId}/Details | Get wish list details
[**get_cart_wish_list_items_async**](WishListsApi.md#get_cart_wish_list_items_async) | **GET** /api/v2/CartService/WishLists/{wishListId}/Records | Get wish list item records
[**get_wish_list_async**](WishListsApi.md#get_wish_list_async) | **GET** /api/v2/CartService/WishLists/{cartId} | Get wish lists for a cart
[**is_product_in_wish_lists**](WishListsApi.md#is_product_in_wish_lists) | **GET** /api/v2/CartService/WishLists/Contains | Check if a product is in any wish list
[**update_product_to_wish_list**](WishListsApi.md#update_product_to_wish_list) | **PUT** /api/v2/CartService/WishLists/{wishListId} | Update a wish list
[**wish_list_exists**](WishListsApi.md#wish_list_exists) | **GET** /api/v2/CartService/WishLists/Exists | Check if a wish list exists
[**wish_list_exists_head_async**](WishListsApi.md#wish_list_exists_head_async) | **HEAD** /api/v2/CartService/WishLists/Exists | Check if a wish list exists (HEAD)



## add_product_to_wish_list

> models::EmptyEnvelope add_product_to_wish_list(api_version, x_api_version, product_to_wish_list_request)
Add a product to a wish list

Adds the specified product to the given wish list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**product_to_wish_list_request** | Option<[**ProductToWishListRequest**](ProductToWishListRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wish_list

> models::EmptyEnvelope create_wish_list(api_version, x_api_version, new_wish_list_request)
Create a wish list

Creates a new wish list from the provided request data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**new_wish_list_request** | Option<[**NewWishListRequest**](NewWishListRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_wish_list

> models::EmptyEnvelope delete_wish_list(wish_list_id, api_version, x_api_version)
Delete a wish list

Deletes the specified wish list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | **uuid::Uuid** |  | [required] |
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


## delete_wish_list_record

> delete_wish_list_record(record_id, api_version, x_api_version)
Delete a wish list record

Removes a specific item record from a wish list by its record ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cart_wish_list_details_async

> models::WishListDto get_cart_wish_list_details_async(wish_list_id, api_version, x_api_version)
Get wish list details

Retrieves the full details of the specified wish list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WishListDto**](WishListDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cart_wish_list_items_async

> Vec<models::WishListItemRecordDto> get_cart_wish_list_items_async(wish_list_id, api_version, x_api_version)
Get wish list item records

Retrieves all item records in the specified wish list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::WishListItemRecordDto>**](WishListItemRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wish_list_async

> Vec<models::WishListDto> get_wish_list_async(cart_id, api_version, x_api_version)
Get wish lists for a cart

Retrieves all wish lists associated with the specified cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::WishListDto>**](WishListDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## is_product_in_wish_lists

> models::BooleanEnvelope is_product_in_wish_lists(cart_id, product_id, api_version, x_api_version)
Check if a product is in any wish list

Returns a boolean indicating whether the specified product exists in any wish list of the given cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | Option<**uuid::Uuid**> |  |  |
**product_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_product_to_wish_list

> models::EmptyEnvelope update_product_to_wish_list(wish_list_id, api_version, x_api_version, wish_list_update_dto)
Update a wish list

Updates the specified wish list with the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**wish_list_update_dto** | Option<[**WishListUpdateDto**](WishListUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## wish_list_exists

> models::BooleanEnvelope wish_list_exists(wish_list_id, api_version, x_api_version)
Check if a wish list exists

Returns a boolean indicating whether the specified wish list exists.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## wish_list_exists_head_async

> models::EmptyEnvelope wish_list_exists_head_async(wish_list_id, api_version, x_api_version)
Check if a wish list exists (HEAD)

HEAD request to check whether the specified wish list exists without returning a response body.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wish_list_id** | Option<**uuid::Uuid**> |  |  |
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

