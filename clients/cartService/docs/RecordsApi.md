# \RecordsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_item_to_cart**](RecordsApi.md#add_item_to_cart) | **POST** /api/v2/CartService/Records/AddItem | Add an item to a cart
[**add_product_to_cart_async**](RecordsApi.md#add_product_to_cart_async) | **POST** /api/v2/CartService/Records | Add a product to a cart with tracking
[**clear_cart_async**](RecordsApi.md#clear_cart_async) | **POST** /api/v2/CartService/Records/ClearCart | Clear all items from a cart
[**decrease_item_cart_record**](RecordsApi.md#decrease_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId}/Decrease | Decrease cart record quantity
[**get_item_cart_record**](RecordsApi.md#get_item_cart_record) | **GET** /api/v2/CartService/Records/{recordId}/Details | Get a cart record by ID
[**get_items_in_cart_async**](RecordsApi.md#get_items_in_cart_async) | **GET** /api/v2/CartService/Records/{cartId} | Get all items in a cart
[**increase_item_cart_record**](RecordsApi.md#increase_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId}/Increase | Increase cart record quantity
[**is_item_already_in_cart**](RecordsApi.md#is_item_already_in_cart) | **GET** /api/v2/CartService/Records/IsInCart | Check if an item is in a cart
[**remove_product_from_cart_by_params**](RecordsApi.md#remove_product_from_cart_by_params) | **DELETE** /api/v2/CartService/Records | Remove a product from a cart
[**remove_product_from_cart_by_record_id**](RecordsApi.md#remove_product_from_cart_by_record_id) | **DELETE** /api/v2/CartService/Records/{recordId} | Remove a product from a cart by record ID
[**update_item_cart_record**](RecordsApi.md#update_item_cart_record) | **PUT** /api/v2/CartService/Records/{recordId} | Update a cart record



## add_item_to_cart

> models::EmptyEnvelope add_item_to_cart(cart_id, item_id, quantity, api_version, x_api_version)
Add an item to a cart

Adds an item with the specified quantity to the given cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | Option<**uuid::Uuid**> |  |  |
**item_id** | Option<**uuid::Uuid**> |  |  |
**quantity** | Option<**i32**> |  |  |
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


## add_product_to_cart_async

> models::EmptyEnvelope add_product_to_cart_async(api_version, x_api_version, item_cart_record_create_dto)
Add a product to a cart with tracking

Adds a product to the cart using a request body with cart ID, product ID, and quantity.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_cart_record_create_dto** | Option<[**ItemCartRecordCreateDto**](ItemCartRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## clear_cart_async

> models::EmptyEnvelope clear_cart_async(cart_id, api_version, x_api_version)
Clear all items from a cart

Removes all item records from the specified cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |
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


## decrease_item_cart_record

> models::EmptyEnvelope decrease_item_cart_record(record_id, quantity, api_version, x_api_version)
Decrease cart record quantity

Decreases the quantity of the specified item cart record by the given amount.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**quantity** | Option<**f64**> |  |  |[default to 1]
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


## get_item_cart_record

> models::EmptyEnvelope get_item_cart_record(record_id, api_version, x_api_version)
Get a cart record by ID

Retrieves the details of a specific item cart record.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
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


## get_items_in_cart_async

> models::ItemCartRecordDtoListEnvelope get_items_in_cart_async(cart_id, api_version, x_api_version)
Get all items in a cart

Retrieves all item cart records for the specified cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCartRecordDtoListEnvelope**](ItemCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## increase_item_cart_record

> models::EmptyEnvelope increase_item_cart_record(record_id, quantity, api_version, x_api_version)
Increase cart record quantity

Increases the quantity of the specified item cart record by the given amount.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**quantity** | Option<**f64**> |  |  |[default to 1]
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


## is_item_already_in_cart

> models::BooleanEnvelope is_item_already_in_cart(item_id, cart_id, api_version, x_api_version)
Check if an item is in a cart

Returns a boolean indicating whether the specified item is already in the given cart.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**cart_id** | **uuid::Uuid** |  | [required] |
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


## remove_product_from_cart_by_params

> models::EmptyEnvelope remove_product_from_cart_by_params(cart_id, product_id, api_version, x_api_version)
Remove a product from a cart

Removes a product from the cart using cart ID and product ID query parameters.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | Option<**uuid::Uuid**> |  |  |
**product_id** | Option<**uuid::Uuid**> |  |  |
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


## remove_product_from_cart_by_record_id

> models::EmptyEnvelope remove_product_from_cart_by_record_id(record_id, api_version, x_api_version)
Remove a product from a cart by record ID

Removes a specific item record from the cart by its record ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
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


## update_item_cart_record

> models::EmptyEnvelope update_item_cart_record(record_id, api_version, x_api_version, item_cart_record_update_dto)
Update a cart record

Updates the specified item cart record with the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**record_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_cart_record_update_dto** | Option<[**ItemCartRecordUpdateDto**](ItemCartRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

