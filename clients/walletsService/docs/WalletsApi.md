# \WalletsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_wallet_bank_account_async**](WalletsApi.md#create_wallet_bank_account_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts | Create Wallet Bank Account
[**create_wallet_location_async**](WalletsApi.md#create_wallet_location_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/Locations | Create Wallet Location
[**create_wallet_payment_async**](WalletsApi.md#create_wallet_payment_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/Payments | Create Wallet Payment
[**create_wallet_token_async**](WalletsApi.md#create_wallet_token_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/Tokens | Create Wallet Token
[**create_wallet_withdraw_request_async**](WalletsApi.md#create_wallet_withdraw_request_async) | **POST** /api/v2/WalletsService/Wallets/{walletId}/Withdraws | Create Wallet Withdraw Request
[**delete_wallet_bank_account_async**](WalletsApi.md#delete_wallet_bank_account_async) | **DELETE** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts/{bankAccountId} | Delete Wallet Bank Account
[**delete_wallet_location_async**](WalletsApi.md#delete_wallet_location_async) | **DELETE** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Delete Wallet Location
[**delete_wallet_token_async**](WalletsApi.md#delete_wallet_token_async) | **DELETE** /api/v2/WalletsService/Wallets/{walletId}/Tokens/{tokenId} | Delete Wallet Token
[**get_incoming_payments_async**](WalletsApi.md#get_incoming_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Incoming | Get Incoming Payments
[**get_incoming_payments_count_async**](WalletsApi.md#get_incoming_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Incoming/Count | Get Incoming Payments Count
[**get_incoming_wallet_invoices_async**](WalletsApi.md#get_incoming_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Incoming | Get Incoming Wallet Invoices
[**get_incoming_wallet_invoices_count_async**](WalletsApi.md#get_incoming_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Incoming/Count | Get Incoming Wallet Invoices Count
[**get_outgoing_payments_async**](WalletsApi.md#get_outgoing_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Outgoing | Get Outgoing Payments
[**get_outgoing_payments_count_async**](WalletsApi.md#get_outgoing_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Outgoing/Count | Get Outgoing Payments Count
[**get_outgoing_wallet_invoices_async**](WalletsApi.md#get_outgoing_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Outgoing | Get Outgoing Wallet Invoices
[**get_outgoing_wallet_invoices_count_async**](WalletsApi.md#get_outgoing_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Outgoing/Count | Get Outgoing Wallet Invoices Count
[**get_wallet_bank_account_async**](WalletsApi.md#get_wallet_bank_account_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts/{bankAccountId} | Get Wallet Bank Account
[**get_wallet_bank_accounts_async**](WalletsApi.md#get_wallet_bank_accounts_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts | Get Wallet Bank Accounts
[**get_wallet_bank_accounts_count_async**](WalletsApi.md#get_wallet_bank_accounts_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts/Count | Get Wallet Bank Accounts Count
[**get_wallet_chargebacks_async**](WalletsApi.md#get_wallet_chargebacks_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Chargebacks | Get Wallet Chargebacks
[**get_wallet_chargebacks_count_async**](WalletsApi.md#get_wallet_chargebacks_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Chargebacks/Count | Get Wallet Chargebacks Count
[**get_wallet_details_async**](WalletsApi.md#get_wallet_details_async) | **GET** /api/v2/WalletsService/Wallets/{walletId} | Get Wallet Details
[**get_wallet_extended_orders_async**](WalletsApi.md#get_wallet_extended_orders_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders/Extended | Get Wallet Extended Orders
[**get_wallet_invoices_async**](WalletsApi.md#get_wallet_invoices_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices | Get Wallet Invoices
[**get_wallet_invoices_count_async**](WalletsApi.md#get_wallet_invoices_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Invoices/Count | Get Wallet Invoices Count
[**get_wallet_location_async**](WalletsApi.md#get_wallet_location_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Get Wallet Location
[**get_wallet_locations_async**](WalletsApi.md#get_wallet_locations_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations | Get Wallet Locations
[**get_wallet_locations_count_async**](WalletsApi.md#get_wallet_locations_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Locations/Count | Get Wallet Locations Count
[**get_wallet_orders_async**](WalletsApi.md#get_wallet_orders_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders | Get Wallet Orders
[**get_wallet_orders_count_async**](WalletsApi.md#get_wallet_orders_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Orders/Count | Get Wallet Orders Count
[**get_wallet_payments_async**](WalletsApi.md#get_wallet_payments_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments | Get Wallet Payments
[**get_wallet_payments_count_async**](WalletsApi.md#get_wallet_payments_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Payments/Count | Get Wallet Payments Count
[**get_wallet_quotes_async**](WalletsApi.md#get_wallet_quotes_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Quotes | Get Wallet Quotes
[**get_wallet_quotes_count_async**](WalletsApi.md#get_wallet_quotes_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Quotes/Count | Get Wallet Quotes Count
[**get_wallet_refunds_async**](WalletsApi.md#get_wallet_refunds_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Refunds | Get Wallet Refunds
[**get_wallet_refunds_count_async**](WalletsApi.md#get_wallet_refunds_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Refunds/Count | Get Wallet Refunds Count
[**get_wallet_token_async**](WalletsApi.md#get_wallet_token_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Tokens/{tokenId} | Get Wallet Token
[**get_wallet_tokens_async**](WalletsApi.md#get_wallet_tokens_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Tokens | Get Wallet Tokens
[**get_wallet_tokens_count_async**](WalletsApi.md#get_wallet_tokens_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Tokens/Count | Get Wallet Tokens Count
[**get_wallet_withdraw_requests_async**](WalletsApi.md#get_wallet_withdraw_requests_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/WithdrawRequests | Get Wallet Withdraw Requests
[**get_wallet_withdraw_requests_count_async**](WalletsApi.md#get_wallet_withdraw_requests_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/WithdrawRequests/Count | Get Wallet Withdraw Requests Count
[**get_wallet_withdraws_async**](WalletsApi.md#get_wallet_withdraws_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Withdraws | Get Wallet Withdraws
[**get_wallet_withdraws_count_async**](WalletsApi.md#get_wallet_withdraws_count_async) | **GET** /api/v2/WalletsService/Wallets/{walletId}/Withdraws/Count | Get Wallet Withdraws Count
[**update_wallet_bank_account_async**](WalletsApi.md#update_wallet_bank_account_async) | **PUT** /api/v2/WalletsService/Wallets/{walletId}/BankAccounts/{bankAccountId} | Update Wallet Bank Account
[**update_wallet_location_async**](WalletsApi.md#update_wallet_location_async) | **PUT** /api/v2/WalletsService/Wallets/{walletId}/Locations/{locationId} | Update Wallet Location
[**update_wallet_token_async**](WalletsApi.md#update_wallet_token_async) | **PUT** /api/v2/WalletsService/Wallets/{walletId}/Tokens/{tokenId} | Update Wallet Token



## create_wallet_bank_account_async

> models::EmptyEnvelope create_wallet_bank_account_async(wallet_id, api_version, x_api_version, bank_account_create_dto)
Create Wallet Bank Account

Create a new bank account for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bank_account_create_dto** | Option<[**BankAccountCreateDto**](BankAccountCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wallet_location_async

> models::EmptyEnvelope create_wallet_location_async(wallet_id, api_version, x_api_version, location_create_dto)
Create Wallet Location

Create a new location for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**location_create_dto** | Option<[**LocationCreateDto**](LocationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wallet_payment_async

> models::EmptyEnvelope create_wallet_payment_async(wallet_id, api_version, x_api_version, payment_create_dto)
Create Wallet Payment

Create a new payment for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_create_dto** | Option<[**PaymentCreateDto**](PaymentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wallet_token_async

> models::EmptyEnvelope create_wallet_token_async(wallet_id, api_version, x_api_version, payment_token_create_dto)
Create Wallet Token

Create a new payment token for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_token_create_dto** | Option<[**PaymentTokenCreateDto**](PaymentTokenCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_wallet_withdraw_request_async

> models::EmptyEnvelope create_wallet_withdraw_request_async(wallet_id, api_version, x_api_version, wallet_withdraw_request_create_dto)
Create Wallet Withdraw Request

Create a new withdraw request for a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**wallet_withdraw_request_create_dto** | Option<[**WalletWithdrawRequestCreateDto**](WalletWithdrawRequestCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_wallet_bank_account_async

> models::EmptyEnvelope delete_wallet_bank_account_async(wallet_id, bank_account_id, api_version, x_api_version)
Delete Wallet Bank Account

Delete a specific bank account of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**bank_account_id** | **uuid::Uuid** |  | [required] |
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


## delete_wallet_location_async

> models::EmptyEnvelope delete_wallet_location_async(wallet_id, location_id, api_version, x_api_version)
Delete Wallet Location

Delete a specific location of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |
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


## delete_wallet_token_async

> models::EmptyEnvelope delete_wallet_token_async(wallet_id, token_id, api_version, x_api_version)
Delete Wallet Token

Delete a specific payment token of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**token_id** | **uuid::Uuid** |  | [required] |
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


## get_incoming_payments_async

> models::PaymentDtoListEnvelope get_incoming_payments_async(wallet_id, api_version, x_api_version)
Get Incoming Payments

Get incoming payments of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_incoming_payments_count_async

> models::Int32Envelope get_incoming_payments_count_async(wallet_id, api_version, x_api_version)
Get Incoming Payments Count

Get incoming payments count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_incoming_wallet_invoices_async

> models::InvoiceDtoListEnvelope get_incoming_wallet_invoices_async(wallet_id, api_version, x_api_version)
Get Incoming Wallet Invoices

Get incoming invoices of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_incoming_wallet_invoices_count_async

> models::Int32Envelope get_incoming_wallet_invoices_count_async(wallet_id, api_version, x_api_version)
Get Incoming Wallet Invoices Count

Get incoming invoices count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_outgoing_payments_async

> models::PaymentDtoListEnvelope get_outgoing_payments_async(wallet_id, api_version, x_api_version)
Get Outgoing Payments

Get outgoing payments of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outgoing_payments_count_async

> models::Int32Envelope get_outgoing_payments_count_async(wallet_id, api_version, x_api_version)
Get Outgoing Payments Count

Get outgoing payments count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_outgoing_wallet_invoices_async

> models::InvoiceDtoListEnvelope get_outgoing_wallet_invoices_async(wallet_id, api_version, x_api_version)
Get Outgoing Wallet Invoices

Get outgoing invoices of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_outgoing_wallet_invoices_count_async

> models::Int32Envelope get_outgoing_wallet_invoices_count_async(wallet_id, api_version, x_api_version)
Get Outgoing Wallet Invoices Count

Get outgoing invoices count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_bank_account_async

> models::BankAccountDtoEnvelope get_wallet_bank_account_async(wallet_id, bank_account_id, api_version, x_api_version)
Get Wallet Bank Account

Get a specific bank account of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**bank_account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BankAccountDtoEnvelope**](BankAccountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_bank_accounts_async

> models::BankAccountDtoListEnvelope get_wallet_bank_accounts_async(wallet_id, api_version, x_api_version)
Get Wallet Bank Accounts

Get bank accounts of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BankAccountDtoListEnvelope**](BankAccountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_bank_accounts_count_async

> models::Int32Envelope get_wallet_bank_accounts_count_async(wallet_id, api_version, x_api_version)
Get Wallet Bank Accounts Count

Get bank accounts count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_chargebacks_async

> models::PaymentChargebackDtoListEnvelope get_wallet_chargebacks_async(wallet_id, api_version, x_api_version)
Get Wallet Chargebacks

Get chargebacks of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentChargebackDtoListEnvelope**](PaymentChargebackDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_chargebacks_count_async

> models::Int32Envelope get_wallet_chargebacks_count_async(wallet_id, api_version, x_api_version)
Get Wallet Chargebacks Count

Get chargebacks count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_details_async

> models::WalletDtoEnvelope get_wallet_details_async(wallet_id, api_version, x_api_version)
Get Wallet Details

Get details of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_extended_orders_async

> models::ExtendedOrderDtoListEnvelope get_wallet_extended_orders_async(wallet_id, api_version, x_api_version)
Get Wallet Extended Orders

Get extended orders of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedOrderDtoListEnvelope**](ExtendedOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_invoices_async

> models::InvoiceDtoListEnvelope get_wallet_invoices_async(wallet_id, api_version, x_api_version)
Get Wallet Invoices

Get invoices of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_invoices_count_async

> models::Int32Envelope get_wallet_invoices_count_async(wallet_id, api_version, x_api_version)
Get Wallet Invoices Count

Get invoices count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_location_async

> models::LocationDtoEnvelope get_wallet_location_async(wallet_id, location_id, api_version, x_api_version)
Get Wallet Location

Get a specific location of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LocationDtoEnvelope**](LocationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_locations_async

> models::LocationDtoListEnvelope get_wallet_locations_async(wallet_id, api_version, x_api_version)
Get Wallet Locations

Get locations of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LocationDtoListEnvelope**](LocationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_locations_count_async

> models::Int32Envelope get_wallet_locations_count_async(wallet_id, api_version, x_api_version)
Get Wallet Locations Count

Get locations count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_orders_async

> models::OrderDtoListEnvelope get_wallet_orders_async(wallet_id, api_version, x_api_version)
Get Wallet Orders

Get orders of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OrderDtoListEnvelope**](OrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_orders_count_async

> models::Int32Envelope get_wallet_orders_count_async(wallet_id, api_version, x_api_version)
Get Wallet Orders Count

Get orders count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_payments_async

> models::PaymentDtoListEnvelope get_wallet_payments_async(wallet_id, api_version, x_api_version)
Get Wallet Payments

Get payments of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentDtoListEnvelope**](PaymentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_payments_count_async

> models::Int32Envelope get_wallet_payments_count_async(wallet_id, api_version, x_api_version)
Get Wallet Payments Count

Get payments count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_quotes_async

> models::QuoteDtoListEnvelope get_wallet_quotes_async(wallet_id, api_version, x_api_version)
Get Wallet Quotes

Get quotes of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::QuoteDtoListEnvelope**](QuoteDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_quotes_count_async

> models::Int32Envelope get_wallet_quotes_count_async(wallet_id, api_version, x_api_version)
Get Wallet Quotes Count

Get quotes count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_refunds_async

> models::PaymentRefundDtoListEnvelope get_wallet_refunds_async(wallet_id, api_version, x_api_version)
Get Wallet Refunds

Get refunds of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentRefundDtoListEnvelope**](PaymentRefundDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_refunds_count_async

> models::Int32Envelope get_wallet_refunds_count_async(wallet_id, api_version, x_api_version)
Get Wallet Refunds Count

Get refunds count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_token_async

> models::PaymentTokenDtoEnvelope get_wallet_token_async(wallet_id, token_id, api_version, x_api_version)
Get Wallet Token

Get a specific payment token of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**token_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentTokenDtoEnvelope**](PaymentTokenDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_tokens_async

> models::PaymentTokenDtoListEnvelope get_wallet_tokens_async(wallet_id, api_version, x_api_version)
Get Wallet Tokens

Get payment tokens of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PaymentTokenDtoListEnvelope**](PaymentTokenDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_tokens_count_async

> models::Int32Envelope get_wallet_tokens_count_async(wallet_id, api_version, x_api_version)
Get Wallet Tokens Count

Get payment tokens count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_withdraw_requests_async

> models::WalletWithdrawRequestDtoListEnvelope get_wallet_withdraw_requests_async(wallet_id, api_version, x_api_version)
Get Wallet Withdraw Requests

Get withdraw requests of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletWithdrawRequestDtoListEnvelope**](WalletWithdrawRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_withdraw_requests_count_async

> models::Int32Envelope get_wallet_withdraw_requests_count_async(wallet_id, api_version, x_api_version)
Get Wallet Withdraw Requests Count

Get withdraw requests count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## get_wallet_withdraws_async

> models::WalletWithdrawDtoListEnvelope get_wallet_withdraws_async(wallet_id, api_version, x_api_version)
Get Wallet Withdraws

Get withdraws of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletWithdrawDtoListEnvelope**](WalletWithdrawDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_wallet_withdraws_count_async

> models::Int32Envelope get_wallet_withdraws_count_async(wallet_id, api_version, x_api_version)
Get Wallet Withdraws Count

Get withdraws count of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
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


## update_wallet_bank_account_async

> models::EmptyEnvelope update_wallet_bank_account_async(wallet_id, bank_account_id, api_version, x_api_version, bank_account_update_dto)
Update Wallet Bank Account

Update a specific bank account of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**bank_account_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**bank_account_update_dto** | Option<[**BankAccountUpdateDto**](BankAccountUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_wallet_location_async

> models::EmptyEnvelope update_wallet_location_async(wallet_id, location_id, api_version, x_api_version, location_update_dto)
Update Wallet Location

Update a specific location of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**location_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**location_update_dto** | Option<[**LocationUpdateDto**](LocationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_wallet_token_async

> models::EmptyEnvelope update_wallet_token_async(wallet_id, token_id, api_version, x_api_version, payment_token_update_dto)
Update Wallet Token

Update a specific payment token of a specific wallet by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**wallet_id** | **uuid::Uuid** |  | [required] |
**token_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**payment_token_update_dto** | Option<[**PaymentTokenUpdateDto**](PaymentTokenUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

