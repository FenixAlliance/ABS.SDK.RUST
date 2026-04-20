# \QuotesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_quote**](QuotesApi.md#calculate_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Calculate | Calculate a quote.
[**calculate_quote_line**](QuotesApi.md#calculate_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId}/Calculate | Calculate a quote line.
[**close_quote**](QuotesApi.md#close_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Close | Close a quote.
[**create_order_from_quote**](QuotesApi.md#create_order_from_quote) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Orders | Create an order from a quote.
[**create_quote**](QuotesApi.md#create_quote) | **POST** /api/v2/QuotesService/Quotes | Create a new quote.
[**create_quote_line**](QuotesApi.md#create_quote_line) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Lines | Create a new quote line.
[**delete_quote**](QuotesApi.md#delete_quote) | **DELETE** /api/v2/QuotesService/Quotes/{quoteId} | Delete a quote.
[**delete_quote_line**](QuotesApi.md#delete_quote_line) | **DELETE** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Delete a quote line.
[**get_extended_quotes**](QuotesApi.md#get_extended_quotes) | **GET** /api/v2/QuotesService/Quotes/Extended | Get a list of extended quotes.
[**get_quote**](QuotesApi.md#get_quote) | **GET** /api/v2/QuotesService/Quotes/{quoteId} | Get a quote by ID.
[**get_quote_line**](QuotesApi.md#get_quote_line) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Get a quote line by ID.
[**get_quote_lines**](QuotesApi.md#get_quote_lines) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines | Get quote lines for a quote.
[**get_quote_lines_count**](QuotesApi.md#get_quote_lines_count) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/Count | Get the count of quote lines.
[**get_quotes**](QuotesApi.md#get_quotes) | **GET** /api/v2/QuotesService/Quotes | Get a list of quotes.
[**get_quotes_count**](QuotesApi.md#get_quotes_count) | **GET** /api/v2/QuotesService/Quotes/Count | Get the count of quotes.
[**preview_quote_email_template**](QuotesApi.md#preview_quote_email_template) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Emails/Preview | Preview the rendered email for an invoice.
[**quote_line_exists**](QuotesApi.md#quote_line_exists) | **GET** /api/v2/QuotesService/Quotes/{quoteId}/Lines/Exists | Check if a quote line exists.
[**reopen_quote**](QuotesApi.md#reopen_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Reopen | Reopen a closed quote.
[**send_quote_email**](QuotesApi.md#send_quote_email) | **POST** /api/v2/QuotesService/Quotes/{quoteId}/Emails/Send | Send a quote transactional email to recipients.
[**update_quote**](QuotesApi.md#update_quote) | **PUT** /api/v2/QuotesService/Quotes/{quoteId} | Update an existing quote.
[**update_quote_line**](QuotesApi.md#update_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId} | Update a quote line.
[**upsert_quote_line**](QuotesApi.md#upsert_quote_line) | **PUT** /api/v2/QuotesService/Quotes/{quoteId}/Lines/{quoteLineId}/Upsert | Upsert a quote line.



## calculate_quote

> models::EmptyEnvelope calculate_quote(tenant_id, quote_id)
Calculate a quote.

Performs calculation logic for the specified quote.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## calculate_quote_line

> models::EmptyEnvelope calculate_quote_line(tenant_id, quote_id, quote_line_id)
Calculate a quote line.

Performs calculation logic for the specified quote line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## close_quote

> models::EmptyEnvelope close_quote(tenant_id, quote_id)
Close a quote.

Closes the specified quote for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_order_from_quote

> models::EmptyEnvelope create_order_from_quote(tenant_id, quote_id)
Create an order from a quote.

Creates an order based on the specified quote for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_quote

> models::EmptyEnvelope create_quote(tenant_id, quote_create_dto)
Create a new quote.

Creates a new quote for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_create_dto** | Option<[**QuoteCreateDto**](QuoteCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_quote_line

> models::EmptyEnvelope create_quote_line(tenant_id, quote_id, quote_line_create_dto)
Create a new quote line.

Creates a new quote line for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_create_dto** | Option<[**QuoteLineCreateDto**](QuoteLineCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_quote

> models::EmptyEnvelope delete_quote(quote_id, tenant_id)
Delete a quote.

Deletes the specified quote for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**quote_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_quote_line

> models::EmptyEnvelope delete_quote_line(tenant_id, quote_id, quote_line_id)
Delete a quote line.

Deletes the specified quote line for the quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_quotes

> models::ExtendedQuoteDtoListEnvelope get_extended_quotes(tenant_id)
Get a list of extended quotes.

Retrieves a list of extended quotes for the specified tenant, supporting OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedQuoteDtoListEnvelope**](ExtendedQuoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quote

> models::QuoteDtoEnvelope get_quote(tenant_id, quote_id)
Get a quote by ID.

Retrieves a single quote by its unique identifier for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::QuoteDtoEnvelope**](QuoteDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quote_line

> models::QuoteLineDtoEnvelope get_quote_line(tenant_id, quote_id, quote_line_id)
Get a quote line by ID.

Retrieves a single quote line by its unique identifier for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::QuoteLineDtoEnvelope**](QuoteLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quote_lines

> models::QuoteLineDtoListEnvelope get_quote_lines(tenant_id, quote_id, item_id)
Get quote lines for a quote.

Retrieves all quote lines for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::QuoteLineDtoListEnvelope**](QuoteLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quote_lines_count

> models::Int32Envelope get_quote_lines_count(tenant_id, quote_id)
Get the count of quote lines.

Retrieves the total count of quote lines for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quotes

> models::QuoteDtoListEnvelope get_quotes(tenant_id)
Get a list of quotes.

Retrieves a list of quotes for the specified tenant, supporting OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::QuoteDtoListEnvelope**](QuoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_quotes_count

> models::Int32Envelope get_quotes_count(tenant_id)
Get the count of quotes.

Retrieves the total count of quotes for the specified tenant, supporting OData query options.

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


## preview_quote_email_template

> preview_quote_email_template(quote_id, tenant_id, email_dispatch_request)
Preview the rendered email for an invoice.

This action is only available for users with the 'send_email' permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**quote_id** | **uuid::Uuid** |  | [required] |
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


## quote_line_exists

> models::BooleanEnvelope quote_line_exists(tenant_id, quote_id, quote_line_id, item_id)
Check if a quote line exists.

Checks if a quote line exists for the specified quote and tenant, by quote line ID or item ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | Option<**uuid::Uuid**> |  |  |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## reopen_quote

> models::EmptyEnvelope reopen_quote(tenant_id, quote_id)
Reopen a closed quote.

Reopens a previously closed quote for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_quote_email

> models::EmptyEnvelope send_quote_email(tenant_id, quote_id, email_dispatch_request)
Send a quote transactional email to recipients.

This action is only available for users with the 'send_email' permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_quote

> models::EmptyEnvelope update_quote(tenant_id, quote_id, quote_update_dto)
Update an existing quote.

Updates an existing quote for the specified tenant and quote ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_update_dto** | Option<[**QuoteUpdateDto**](QuoteUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_quote_line

> models::EmptyEnvelope update_quote_line(tenant_id, quote_id, quote_line_id, quote_line_update_dto)
Update a quote line.

Updates an existing quote line for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | **uuid::Uuid** |  | [required] |
**quote_line_update_dto** | Option<[**QuoteLineUpdateDto**](QuoteLineUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upsert_quote_line

> models::EmptyEnvelope upsert_quote_line(tenant_id, quote_id, quote_line_id, quote_line_upsert_dto)
Upsert a quote line.

Creates or updates a quote line for the specified quote and tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**quote_id** | **uuid::Uuid** |  | [required] |
**quote_line_id** | **uuid::Uuid** |  | [required] |
**quote_line_upsert_dto** | Option<[**QuoteLineUpsertDto**](QuoteLineUpsertDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

