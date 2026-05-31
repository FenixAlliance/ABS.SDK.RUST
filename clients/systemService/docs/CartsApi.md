# \CartsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_system_cart**](CartsApi.md#delete_system_cart) | **DELETE** /api/v2/SystemService/Carts/{cartId} | Delete a system cart
[**get_system_cart_by_id**](CartsApi.md#get_system_cart_by_id) | **GET** /api/v2/SystemService/Carts/{cartId} | Retrieve a single system cart by its ID
[**get_system_carts**](CartsApi.md#get_system_carts) | **GET** /api/v2/SystemService/Carts | Retrieve a list of system carts
[**get_system_carts_count**](CartsApi.md#get_system_carts_count) | **GET** /api/v2/SystemService/Carts/Count | Get the count of system carts



## delete_system_cart

> models::EmptyEnvelope delete_system_cart(cart_id, api_version, x_api_version)
Delete a system cart

Delete a system cart by its ID

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


## get_system_cart_by_id

> models::CartDtoEnvelope get_system_cart_by_id(cart_id, api_version, x_api_version)
Retrieve a single system cart by its ID

Retrieve a single system cart by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_carts

> models::CartDtoListEnvelope get_system_carts(api_version, x_api_version)
Retrieve a list of system carts

Retrieve a list of all carts in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CartDtoListEnvelope**](CartDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_carts_count

> models::Int32Envelope get_system_carts_count(api_version, x_api_version)
Get the count of system carts

Get the count of all carts in the system

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
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

