# \InvoicesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aggregate_invoice_discounts**](InvoicesApi.md#aggregate_invoice_discounts) | **POST** /api/v2/InvoicingService/Invoices/DiscountsAggregate | Aggregate invoice discounts.
[**aggregate_invoice_global_surcharges**](InvoicesApi.md#aggregate_invoice_global_surcharges) | **POST** /api/v2/InvoicingService/Invoices/GlobalSurchargesAggregate | Aggregate invoice global surcharges.
[**aggregate_invoice_tax_bases**](InvoicesApi.md#aggregate_invoice_tax_bases) | **POST** /api/v2/InvoicingService/Invoices/TaxBasesAggregate | Aggregate invoice tax bases.
[**aggregate_invoice_taxes**](InvoicesApi.md#aggregate_invoice_taxes) | **POST** /api/v2/InvoicingService/Invoices/TaxesAggregate | Aggregate invoice taxes.
[**aggregate_invoice_totals**](InvoicesApi.md#aggregate_invoice_totals) | **POST** /api/v2/InvoicingService/Invoices/TotalsAggregate | Aggregate invoice totals.
[**calculate_invoice**](InvoicesApi.md#calculate_invoice) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Calculate | Calculate an invoice.
[**calculate_invoice_line**](InvoicesApi.md#calculate_invoice_line) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Calculate | Calculate an invoice line.
[**create_invoice**](InvoicesApi.md#create_invoice) | **POST** /api/v2/InvoicingService/Invoices | Create a new invoice.
[**create_invoice_adjustment**](InvoicesApi.md#create_invoice_adjustment) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments | Create a new invoice adjustment.
[**create_invoice_line**](InvoicesApi.md#create_invoice_line) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines | Create a new invoice line.
[**create_invoice_line_tax**](InvoicesApi.md#create_invoice_line_tax) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes | Create a new tax for an invoice line.
[**create_invoice_reference**](InvoicesApi.md#create_invoice_reference) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/References | Create a new invoice reference.
[**delete_invoice**](InvoicesApi.md#delete_invoice) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId} | Delete an invoice.
[**delete_invoice_adjustment**](InvoicesApi.md#delete_invoice_adjustment) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Delete an invoice adjustment.
[**delete_invoice_line**](InvoicesApi.md#delete_invoice_line) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Delete an invoice line.
[**delete_invoice_line_tax**](InvoicesApi.md#delete_invoice_line_tax) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/{invoiceLineTaxId} | Delete a tax from an invoice line.
[**delete_invoice_reference**](InvoicesApi.md#delete_invoice_reference) | **DELETE** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Delete an invoice reference.
[**get_extended_invoice**](InvoicesApi.md#get_extended_invoice) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Extended | Get an extended invoice by ID.
[**get_extended_invoices**](InvoicesApi.md#get_extended_invoices) | **GET** /api/v2/InvoicingService/Invoices/Extended | Get a list of extended invoices.
[**get_extended_invoices_count**](InvoicesApi.md#get_extended_invoices_count) | **GET** /api/v2/InvoicingService/Invoices/Extended/Count | Get the count of extended invoices.
[**get_invoice**](InvoicesApi.md#get_invoice) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId} | Get an invoice by ID.
[**get_invoice_adjustment**](InvoicesApi.md#get_invoice_adjustment) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Get an invoice adjustment by ID.
[**get_invoice_adjustments**](InvoicesApi.md#get_invoice_adjustments) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments | Get invoice adjustments.
[**get_invoice_adjustments_count**](InvoicesApi.md#get_invoice_adjustments_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/Count | Get the count of invoice adjustments.
[**get_invoice_line**](InvoicesApi.md#get_invoice_line) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Get an invoice line by ID.
[**get_invoice_line_taxes**](InvoicesApi.md#get_invoice_line_taxes) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes | Get taxes for an invoice line.
[**get_invoice_line_taxes_count**](InvoicesApi.md#get_invoice_line_taxes_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/Count | Get the count of taxes for an invoice line.
[**get_invoice_lines**](InvoicesApi.md#get_invoice_lines) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines | Get invoice lines.
[**get_invoice_lines_count**](InvoicesApi.md#get_invoice_lines_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/Count | Get the count of invoice lines.
[**get_invoice_payments**](InvoicesApi.md#get_invoice_payments) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Payments | Get payments for an invoice.
[**get_invoice_payments_count**](InvoicesApi.md#get_invoice_payments_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/Payments/Count | Get the count of payments for an invoice.
[**get_invoice_reference**](InvoicesApi.md#get_invoice_reference) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Get an invoice reference by ID.
[**get_invoice_references**](InvoicesApi.md#get_invoice_references) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References | Get invoice references.
[**get_invoice_references_count**](InvoicesApi.md#get_invoice_references_count) | **GET** /api/v2/InvoicingService/Invoices/{invoiceId}/References/Count | Get the count of invoice references.
[**get_invoices**](InvoicesApi.md#get_invoices) | **GET** /api/v2/InvoicingService/Invoices | Get a list of invoices.
[**get_invoices_count**](InvoicesApi.md#get_invoices_count) | **GET** /api/v2/InvoicingService/Invoices/Count | Get the count of invoices.
[**preview_invoice_email**](InvoicesApi.md#preview_invoice_email) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Emails/Preview | Preview the rendered email for an invoice.
[**send_invoice_email**](InvoicesApi.md#send_invoice_email) | **POST** /api/v2/InvoicingService/Invoices/{invoiceId}/Emails/Send | Send an invoice transactional email to recipients.
[**update_invoice**](InvoicesApi.md#update_invoice) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId} | Update an invoice.
[**update_invoice_adjustment**](InvoicesApi.md#update_invoice_adjustment) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Adjustments/{invoiceAdjustmentId} | Update an invoice adjustment.
[**update_invoice_line**](InvoicesApi.md#update_invoice_line) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId} | Update an invoice line.
[**update_invoice_line_tax**](InvoicesApi.md#update_invoice_line_tax) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/Lines/{invoiceLineId}/Taxes/{invoiceLineTaxId} | Update a tax for an invoice line.
[**update_invoice_reference**](InvoicesApi.md#update_invoice_reference) | **PUT** /api/v2/InvoicingService/Invoices/{invoiceId}/References/{invoiceReferenceId} | Update an invoice reference.



## aggregate_invoice_discounts

> models::MoneyEnvelope aggregate_invoice_discounts(uuid_colon_colon_uuid, currency_id)
Aggregate invoice discounts.

Aggregates the discounts for the specified invoices.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid_colon_colon_uuid** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) |  | [required] |
**currency_id** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## aggregate_invoice_global_surcharges

> models::MoneyEnvelope aggregate_invoice_global_surcharges(uuid_colon_colon_uuid, currency_id)
Aggregate invoice global surcharges.

Aggregates the global surcharges for the specified invoices.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid_colon_colon_uuid** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) |  | [required] |
**currency_id** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## aggregate_invoice_tax_bases

> models::MoneyEnvelope aggregate_invoice_tax_bases(uuid_colon_colon_uuid, currency_id)
Aggregate invoice tax bases.

Aggregates the tax bases for the specified invoices.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid_colon_colon_uuid** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) |  | [required] |
**currency_id** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## aggregate_invoice_taxes

> models::MoneyEnvelope aggregate_invoice_taxes(uuid_colon_colon_uuid, currency_id)
Aggregate invoice taxes.

Aggregates the taxes for the specified invoices.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid_colon_colon_uuid** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) |  | [required] |
**currency_id** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## aggregate_invoice_totals

> models::MoneyEnvelope aggregate_invoice_totals(uuid_colon_colon_uuid, currency_id)
Aggregate invoice totals.

Aggregates the totals for the specified invoices.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid_colon_colon_uuid** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) |  | [required] |
**currency_id** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## calculate_invoice

> models::EmptyEnvelope calculate_invoice(tenant_id, invoice_id)
Calculate an invoice.

Calculates the totals and taxes for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## calculate_invoice_line

> models::EmptyEnvelope calculate_invoice_line(tenant_id, invoice_id, invoice_line_id)
Calculate an invoice line.

Calculates the totals and taxes for the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_invoice

> models::EmptyEnvelope create_invoice(tenant_id, invoice_create_dto)
Create a new invoice.

Creates a new invoice for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_create_dto** | Option<[**InvoiceCreateDto**](InvoiceCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_invoice_adjustment

> models::EmptyEnvelope create_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_create_dto)
Create a new invoice adjustment.

Creates a new adjustment for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_adjustment_create_dto** | Option<[**InvoiceAdjustmentCreateDto**](InvoiceAdjustmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_invoice_line

> models::InvoiceLineDtoIReadOnlyListEnvelope create_invoice_line(tenant_id, invoice_id, invoice_line_create_dto)
Create a new invoice line.

Creates a new invoice line for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_create_dto** | Option<[**InvoiceLineCreateDto**](InvoiceLineCreateDto.md)> |  |  |

### Return type

[**models::InvoiceLineDtoIReadOnlyListEnvelope**](InvoiceLineDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_invoice_line_tax

> models::EmptyEnvelope create_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_applied_tax_create_dto)
Create a new tax for an invoice line.

Creates a new tax entry for the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |
**invoice_line_applied_tax_create_dto** | Option<[**InvoiceLineAppliedTaxCreateDto**](InvoiceLineAppliedTaxCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_invoice_reference

> models::EmptyEnvelope create_invoice_reference(tenant_id, invoice_id, invoice_reference_create_dto)
Create a new invoice reference.

Creates a new reference for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_reference_create_dto** | Option<[**InvoiceReferenceCreateDto**](InvoiceReferenceCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice

> models::EmptyEnvelope delete_invoice(tenant_id, invoice_id)
Delete an invoice.

Deletes the specified invoice for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice_adjustment

> models::EmptyEnvelope delete_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)
Delete an invoice adjustment.

Deletes the specified adjustment from the invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_adjustment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice_line

> models::EmptyEnvelope delete_invoice_line(tenant_id, invoice_id, invoice_line_id)
Delete an invoice line.

Deletes the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice_line_tax

> models::EmptyEnvelope delete_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id)
Delete a tax from an invoice line.

Deletes the specified tax entry from the invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |
**invoice_line_tax_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_invoice_reference

> models::EmptyEnvelope delete_invoice_reference(tenant_id, invoice_id, invoice_reference_id)
Delete an invoice reference.

Deletes the specified reference from the invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_reference_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_invoice

> models::InvoiceDtoEnvelope get_extended_invoice(tenant_id, invoice_id)
Get an extended invoice by ID.

Retrieves the extended invoice details for the specified invoice ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceDtoEnvelope**](InvoiceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_invoices

> models::ExtendedInvoiceDtoListEnvelope get_extended_invoices(tenant_id)
Get a list of extended invoices.

Retrieves a list of extended invoice details for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::ExtendedInvoiceDtoListEnvelope**](ExtendedInvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_invoices_count

> models::Int32Envelope get_extended_invoices_count(tenant_id)
Get the count of extended invoices.

Retrieves the total count of extended invoices for the specified tenant.

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


## get_invoice

> models::InvoiceDtoEnvelope get_invoice(tenant_id, invoice_id)
Get an invoice by ID.

Retrieves the invoice details for the specified invoice ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceDtoEnvelope**](InvoiceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_adjustment

> models::InvoiceAdjustmentDtoEnvelope get_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id)
Get an invoice adjustment by ID.

Retrieves the adjustment details for the specified invoice adjustment ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_adjustment_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceAdjustmentDtoEnvelope**](InvoiceAdjustmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_adjustments

> models::InvoiceAdjustmentDtoIReadOnlyListEnvelope get_invoice_adjustments(tenant_id, invoice_id)
Get invoice adjustments.

Retrieves the adjustments for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceAdjustmentDtoIReadOnlyListEnvelope**](InvoiceAdjustmentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_adjustments_count

> models::Int32Envelope get_invoice_adjustments_count(tenant_id, invoice_id)
Get the count of invoice adjustments.

Retrieves the total count of adjustments for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_line

> models::InvoiceLineDtoEnvelope get_invoice_line(tenant_id, invoice_id, invoice_line_id)
Get an invoice line by ID.

Retrieves the invoice line details for the specified invoice line ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceLineDtoEnvelope**](InvoiceLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_line_taxes

> models::InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope get_invoice_line_taxes(tenant_id, invoice_id, invoice_line_id)
Get taxes for an invoice line.

Retrieves the taxes applied to the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope**](InvoiceLineAppliedTaxDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_line_taxes_count

> models::Int32Envelope get_invoice_line_taxes_count(tenant_id, invoice_id, invoice_line_id)
Get the count of taxes for an invoice line.

Retrieves the total count of taxes applied to the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_lines

> models::InvoiceLineDtoListEnvelope get_invoice_lines(tenant_id, invoice_id, item_id)
Get invoice lines.

Retrieves the invoice lines for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**item_id** | Option<**uuid::Uuid**> |  |  |

### Return type

[**models::InvoiceLineDtoListEnvelope**](InvoiceLineDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_lines_count

> models::Int32Envelope get_invoice_lines_count(tenant_id, invoice_id)
Get the count of invoice lines.

Retrieves the total count of invoice lines for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_payments

> models::PaymentDtoIReadOnlyListEnvelope get_invoice_payments(invoice_id)
Get payments for an invoice.

Retrieves the list of payments related to the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::PaymentDtoIReadOnlyListEnvelope**](PaymentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_payments_count

> models::Int32Envelope get_invoice_payments_count(invoice_id)
Get the count of payments for an invoice.

Retrieves the total count of payments for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_reference

> models::InvoiceReferenceDtoEnvelope get_invoice_reference(tenant_id, invoice_id, invoice_reference_id)
Get an invoice reference by ID.

Retrieves the reference details for the specified invoice reference ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_reference_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceReferenceDtoEnvelope**](InvoiceReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_references

> models::InvoiceReferenceDtoIReadOnlyListEnvelope get_invoice_references(tenant_id, invoice_id)
Get invoice references.

Retrieves the references for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceReferenceDtoIReadOnlyListEnvelope**](InvoiceReferenceDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoice_references_count

> models::Int32Envelope get_invoice_references_count(tenant_id, invoice_id)
Get the count of invoice references.

Retrieves the total count of references for the specified invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoices

> models::InvoiceDtoListEnvelope get_invoices(tenant_id)
Get a list of invoices.

Retrieves a list of invoices for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::InvoiceDtoListEnvelope**](InvoiceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invoices_count

> models::Int32Envelope get_invoices_count(tenant_id)
Get the count of invoices.

Retrieves the total count of invoices for the specified tenant.

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


## preview_invoice_email

> preview_invoice_email(invoice_id, tenant_id, email_dispatch_request)
Preview the rendered email for an invoice.

This action is only available for users with the 'send_email' permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invoice_id** | **uuid::Uuid** |  | [required] |
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


## send_invoice_email

> models::Envelope send_invoice_email(tenant_id, invoice_id, email_dispatch_request)
Send an invoice transactional email to recipients.

This action is only available for users with the 'send_email' permission.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice

> models::EmptyEnvelope update_invoice(tenant_id, invoice_id, invoice_update_dto)
Update an invoice.

Updates the specified invoice for the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_update_dto** | Option<[**InvoiceUpdateDto**](InvoiceUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice_adjustment

> models::EmptyEnvelope update_invoice_adjustment(tenant_id, invoice_id, invoice_adjustment_id, invoice_adjustment_update_dto)
Update an invoice adjustment.

Updates the specified adjustment for the invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_adjustment_id** | **uuid::Uuid** |  | [required] |
**invoice_adjustment_update_dto** | Option<[**InvoiceAdjustmentUpdateDto**](InvoiceAdjustmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice_line

> models::InvoiceLineDtoEnvelope update_invoice_line(tenant_id, invoice_id, invoice_line_id, invoice_line_update_dto)
Update an invoice line.

Updates the specified invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |
**invoice_line_update_dto** | Option<[**InvoiceLineUpdateDto**](InvoiceLineUpdateDto.md)> |  |  |

### Return type

[**models::InvoiceLineDtoEnvelope**](InvoiceLineDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice_line_tax

> models::EmptyEnvelope update_invoice_line_tax(tenant_id, invoice_id, invoice_line_id, invoice_line_tax_id, invoice_line_applied_tax_update_dto)
Update a tax for an invoice line.

Updates the specified tax entry for the invoice line.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_line_id** | **uuid::Uuid** |  | [required] |
**invoice_line_tax_id** | **uuid::Uuid** |  | [required] |
**invoice_line_applied_tax_update_dto** | Option<[**InvoiceLineAppliedTaxUpdateDto**](InvoiceLineAppliedTaxUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_invoice_reference

> models::EmptyEnvelope update_invoice_reference(tenant_id, invoice_id, invoice_reference_id, invoice_reference_update_dto)
Update an invoice reference.

Updates the specified reference for the invoice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**invoice_id** | **uuid::Uuid** |  | [required] |
**invoice_reference_id** | **uuid::Uuid** |  | [required] |
**invoice_reference_update_dto** | Option<[**InvoiceReferenceUpdateDto**](InvoiceReferenceUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

