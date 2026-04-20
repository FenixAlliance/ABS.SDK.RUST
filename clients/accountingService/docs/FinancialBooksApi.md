# \FinancialBooksApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_financial_book_async**](FinancialBooksApi.md#create_financial_book_async) | **POST** /api/v2/AccountingService/FinancialBooks | Creates a new financial book
[**delete_financial_book_async**](FinancialBooksApi.md#delete_financial_book_async) | **DELETE** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Deletes an existing financial book
[**get_financial_book_details_async**](FinancialBooksApi.md#get_financial_book_details_async) | **GET** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Gets the details of a specific financial book
[**get_financial_books_async**](FinancialBooksApi.md#get_financial_books_async) | **GET** /api/v2/AccountingService/FinancialBooks | Get all financial books for a tenant
[**get_financial_books_count_async**](FinancialBooksApi.md#get_financial_books_count_async) | **GET** /api/v2/AccountingService/FinancialBooks/Count | Get the count of financial books
[**update_financial_book_async**](FinancialBooksApi.md#update_financial_book_async) | **PUT** /api/v2/AccountingService/FinancialBooks/{financialBookId} | Updates an existing financial book



## create_financial_book_async

> models::EmptyEnvelope create_financial_book_async(tenant_id, financial_book_create_dto, api_version, x_api_version)
Creates a new financial book

Creates a new financial book.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**financial_book_create_dto** | [**FinancialBookCreateDto**](FinancialBookCreateDto.md) |  | [required] |
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


## delete_financial_book_async

> models::EmptyEnvelope delete_financial_book_async(tenant_id, financial_book_id, api_version, x_api_version)
Deletes an existing financial book

Deletes an existing financial book.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**financial_book_id** | **uuid::Uuid** |  | [required] |
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


## get_financial_book_details_async

> models::FinancialBookDtoEnvelope get_financial_book_details_async(tenant_id, financial_book_id, api_version, x_api_version)
Gets the details of a specific financial book

Gets the details of a specific financial book.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**financial_book_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FinancialBookDtoEnvelope**](FinancialBookDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_financial_books_async

> models::FinancialBookDtoListEnvelope get_financial_books_async(tenant_id, api_version, x_api_version)
Get all financial books for a tenant

Retrieves all financial books for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FinancialBookDtoListEnvelope**](FinancialBookDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_financial_books_count_async

> models::Int32Envelope get_financial_books_count_async(tenant_id, api_version, x_api_version)
Get the count of financial books

Get the count of financial books.

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


## update_financial_book_async

> models::EmptyEnvelope update_financial_book_async(tenant_id, financial_book_id, financial_book_update_dto, api_version, x_api_version)
Updates an existing financial book

Updates an existing financial book.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**financial_book_id** | **uuid::Uuid** |  | [required] |
**financial_book_update_dto** | [**FinancialBookUpdateDto**](FinancialBookUpdateDto.md) |  | [required] |
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

