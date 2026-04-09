# \OrdersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_order**](OrdersApi.md#calculate_order) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Calculate | Calculates totals for an order.
[**calculate_order_line**](OrdersApi.md#calculate_order_line) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId}/Calculate | Calculates totals for an order line.
[**create_order**](OrdersApi.md#create_order) | **POST** /api/v2/OrdersService/Orders | Creates a new order.
[**create_order_line**](OrdersApi.md#create_order_line) | **POST** /api/v2/OrdersService/Orders/{orderId}/Lines | Creates a new order line.
[**delete_order**](OrdersApi.md#delete_order) | **DELETE** /api/v2/OrdersService/Orders/{orderId} | Deletes an order.
[**delete_order_line**](OrdersApi.md#delete_order_line) | **DELETE** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Deletes an order line.
[**get_extended_orders**](OrdersApi.md#get_extended_orders) | **GET** /api/v2/OrdersService/Orders/Extended | Gets a list of extended orders for a tenant.
[**get_order**](OrdersApi.md#get_order) | **GET** /api/v2/OrdersService/Orders/{orderId} | Gets a specific order by ID.
[**get_order_line**](OrdersApi.md#get_order_line) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Gets a specific order line.
[**get_order_lines**](OrdersApi.md#get_order_lines) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines | Gets order lines for an order.
[**get_order_lines_count**](OrdersApi.md#get_order_lines_count) | **GET** /api/v2/OrdersService/Orders/{orderId}/Lines/Count | Gets the count of order lines for an order.
[**get_orders**](OrdersApi.md#get_orders) | **GET** /api/v2/OrdersService/Orders | Gets a list of orders for a tenant.
[**get_orders_count**](OrdersApi.md#get_orders_count) | **GET** /api/v2/OrdersService/Orders/Count | Gets the count of orders for a tenant.
[**preview_order_email_template**](OrdersApi.md#preview_order_email_template) | **POST** /api/v2/OrdersService/Orders/{orderId}/Emails/Preview | Preview the rendered email for an Order.
[**send_order_email**](OrdersApi.md#send_order_email) | **POST** /api/v2/OrdersService/Orders/{orderId}/Emails/Send | Send a transactional email for an order.
[**submit_cart**](OrdersApi.md#submit_cart) | **POST** /api/v2/OrdersService/Orders/SubmitCart | Submits a cart and creates an order.
[**update_order**](OrdersApi.md#update_order) | **PUT** /api/v2/OrdersService/Orders/{orderId} | Updates an existing order.
[**update_order_line**](OrdersApi.md#update_order_line) | **PUT** /api/v2/OrdersService/Orders/{orderId}/Lines/{orderLineId} | Updates an order line.



## calculate_order

> models::EmptyEnvelope calculate_order(tenant_id, order_id)
Calculates totals for an order.

Performs calculation of totals and taxes for the specified order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## calculate_order_line

> models::EmptyEnvelope calculate_order_line(tenant_id, order_id, order_line_id)
Calculates totals for an order line.

Performs calculation of totals and taxes for the specified order line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_order

> models::EmptyEnvelope create_order(tenant_id, order_create_dto)
Creates a new order.

Creates a new order for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_create_dto** | Option<[**OrderCreateDto**](OrderCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_order_line

> models::EmptyEnvelope create_order_line(tenant_id, order_id, order_line_create_dto)
Creates a new order line.

Creates a new line (item) for the specified order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_line_create_dto** | Option<[**OrderLineCreateDto**](OrderLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_order

> models::EmptyEnvelope delete_order(tenant_id, order_id)
Deletes an order.

Deletes the specified order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_order_line

> models::EmptyEnvelope delete_order_line(tenant_id, order_id, order_line_id)
Deletes an order line.

Deletes the specified order line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_orders

> models::ExtendedOrderDtoListEnvelope get_extended_orders(tenant_id)
Gets a list of extended orders for a tenant.

Retrieves a list of extended order details for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedOrderDtoListEnvelope**](ExtendedOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_order

> models::OrderDtoEnvelope get_order(tenant_id, order_id)
Gets a specific order by ID.

Retrieves the details of a specific order by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_order_line

> models::OrderLineDtoEnvelope get_order_line(tenant_id, order_id, order_line_id)
Gets a specific order line.

Retrieves the details of a specific order line by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::OrderLineDtoEnvelope**](OrderLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_order_lines

> models::OrderLineDtoListEnvelope get_order_lines(tenant_id, order_id, item_id)
Gets order lines for an order.

Retrieves the lines (items) for the specified order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::OrderLineDtoListEnvelope**](OrderLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_order_lines_count

> models::Int32Envelope get_order_lines_count(tenant_id, order_id)
Gets the count of order lines for an order.

Retrieves the total number of lines for the specified order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_orders

> models::OrderDtoListEnvelope get_orders(tenant_id)
Gets a list of orders for a tenant.

Retrieves a list of orders for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::OrderDtoListEnvelope**](OrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_orders_count

> models::Int32Envelope get_orders_count(tenant_id)
Gets the count of orders for a tenant.

Retrieves the total number of orders for the specified tenant.

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


## preview_order_email_template

> preview_order_email_template(order_id, tenant_id, email_dispatch_request)
Preview the rendered email for an Order.

Previews the rendered email template for the specified order. Only users with the 'send_email' permission are permitted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**order_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_order_email

> models::EmptyEnvelope send_order_email(tenant_id, order_id, email_dispatch_request)
Send a transactional email for an order.

Sends a transactional email for the specified order. Only users with the 'send_email' permission are permitted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## submit_cart

> models::OrderDtoEnvelope submit_cart(cart_id)
Submits a cart and creates an order.

Submits the specified cart and creates an order for the authenticated user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cart_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_order

> models::EmptyEnvelope update_order(tenant_id, order_id, order_update_dto)
Updates an existing order.

Updates the details of an existing order.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_update_dto** | Option<[**OrderUpdateDto**](OrderUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_order_line

> models::EmptyEnvelope update_order_line(tenant_id, order_id, order_line_id, order_line_update_dto)
Updates an order line.

Updates the details of a specific order line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**order_id** | **uuid::Uuid** |  | [required] |
**order_line_id** | **uuid::Uuid** |  | [required] |
**order_line_update_dto** | Option<[**OrderLineUpdateDto**](OrderLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

