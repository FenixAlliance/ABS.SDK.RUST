# \TransactionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_transaction**](TransactionsApi.md#create_transaction) | **POST** /api/v2/AccountingService/Transactions | Create a transaction
[**create_transaction_category**](TransactionsApi.md#create_transaction_category) | **POST** /api/v2/AccountingService/Transactions/Categories | Create a transaction category
[**delete_transaction**](TransactionsApi.md#delete_transaction) | **DELETE** /api/v2/AccountingService/Transactions/{transactionId} | Delete a transaction
[**delete_transaction_category**](TransactionsApi.md#delete_transaction_category) | **DELETE** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Delete a transaction category
[**get_transaction**](TransactionsApi.md#get_transaction) | **GET** /api/v2/AccountingService/Transactions/{transactionId} | Get transaction by ID
[**get_transaction_categories**](TransactionsApi.md#get_transaction_categories) | **GET** /api/v2/AccountingService/Transactions/Categories | Get all transaction categories
[**get_transaction_categories_count**](TransactionsApi.md#get_transaction_categories_count) | **GET** /api/v2/AccountingService/Transactions/Categories/Count | Get transaction categories count
[**get_transaction_category**](TransactionsApi.md#get_transaction_category) | **GET** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Get transaction category by ID
[**get_transactions**](TransactionsApi.md#get_transactions) | **GET** /api/v2/AccountingService/Transactions | Get all transactions for a tenant
[**get_transactions_count**](TransactionsApi.md#get_transactions_count) | **GET** /api/v2/AccountingService/Transactions/Count | Get transactions count
[**update_transaction**](TransactionsApi.md#update_transaction) | **PUT** /api/v2/AccountingService/Transactions/{transactionId} | Update a transaction
[**update_transaction_category**](TransactionsApi.md#update_transaction_category) | **PUT** /api/v2/AccountingService/Transactions/Categories/{categoryId} | Update a transaction category



## create_transaction

> models::TransactionDtoEnvelope create_transaction(tenant_id, api_version, x_api_version, transaction_create_dto)
Create a transaction

Creates a new transaction for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**transaction_create_dto** | Option<[**TransactionCreateDto**](TransactionCreateDto.md)> |  |  |

### Return type

[**models::TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_transaction_category

> models::TransactionCategoryDtoEnvelope create_transaction_category(tenant_id, api_version, x_api_version, transaction_category_create_dto)
Create a transaction category

Creates a new transaction category for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**transaction_category_create_dto** | Option<[**TransactionCategoryCreateDto**](TransactionCategoryCreateDto.md)> |  |  |

### Return type

[**models::TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_transaction

> models::TransactionDtoEnvelope delete_transaction(tenant_id, transaction_id, api_version, x_api_version)
Delete a transaction

Deletes a transaction by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transaction_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_transaction_category

> models::TransactionCategoryDtoEnvelope delete_transaction_category(tenant_id, category_id, api_version, x_api_version)
Delete a transaction category

Deletes a transaction category by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transaction

> models::TransactionDtoEnvelope get_transaction(tenant_id, transaction_id, api_version, x_api_version)
Get transaction by ID

Retrieves a specific transaction by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transaction_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transaction_categories

> models::TransactionCategoryDtoListEnvelope get_transaction_categories(tenant_id, api_version, x_api_version)
Get all transaction categories

Retrieves all transaction categories for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionCategoryDtoListEnvelope**](TransactionCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transaction_categories_count

> models::Int32Envelope get_transaction_categories_count(tenant_id, api_version, x_api_version)
Get transaction categories count

Returns total number of transaction categories for the tenant.

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


## get_transaction_category

> models::TransactionCategoryDtoEnvelope get_transaction_category(tenant_id, category_id, api_version, x_api_version)
Get transaction category by ID

Retrieves a specific transaction category by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transactions

> models::TransactionDtoListEnvelope get_transactions(tenant_id, api_version, x_api_version)
Get all transactions for a tenant

Retrieves all transactions for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TransactionDtoListEnvelope**](TransactionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transactions_count

> models::Int32Envelope get_transactions_count(tenant_id, api_version, x_api_version)
Get transactions count

Returns total number of transactions for the tenant with OData filter support.

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


## update_transaction

> models::TransactionDtoEnvelope update_transaction(tenant_id, transaction_id, api_version, x_api_version, transaction_update_dto)
Update a transaction

Updates an existing transaction with the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transaction_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**transaction_update_dto** | Option<[**TransactionUpdateDto**](TransactionUpdateDto.md)> |  |  |

### Return type

[**models::TransactionDtoEnvelope**](TransactionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_transaction_category

> models::TransactionCategoryDtoEnvelope update_transaction_category(tenant_id, category_id, api_version, x_api_version, transaction_category_update_dto)
Update a transaction category

Updates an existing transaction category with the provided data.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**transaction_category_update_dto** | Option<[**TransactionCategoryUpdateDto**](TransactionCategoryUpdateDto.md)> |  |  |

### Return type

[**models::TransactionCategoryDtoEnvelope**](TransactionCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

