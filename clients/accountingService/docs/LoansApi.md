# \LoansApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_loan_application_async**](LoansApi.md#create_loan_application_async) | **POST** /api/v2/AccountingService/Loans/Applications | Creates a loan application
[**create_loan_async**](LoansApi.md#create_loan_async) | **POST** /api/v2/AccountingService/Loans | Creates a new loan
[**delete_loan_application_async**](LoansApi.md#delete_loan_application_async) | **DELETE** /api/v2/AccountingService/Loans/Applications/{applicationId} | Deletes a loan application
[**delete_loan_async**](LoansApi.md#delete_loan_async) | **DELETE** /api/v2/AccountingService/Loans/{loanId} | Deletes a loan
[**get_loan_application_details_async**](LoansApi.md#get_loan_application_details_async) | **GET** /api/v2/AccountingService/Loans/Applications/{applicationId} | Gets a loan application by ID
[**get_loan_applications_async**](LoansApi.md#get_loan_applications_async) | **GET** /api/v2/AccountingService/Loans/Applications | Gets all loan applications
[**get_loan_applications_count_async**](LoansApi.md#get_loan_applications_count_async) | **GET** /api/v2/AccountingService/Loans/Applications/Count | Counts loan applications
[**get_loan_details_async**](LoansApi.md#get_loan_details_async) | **GET** /api/v2/AccountingService/Loans/{loanId} | Gets a loan by ID
[**get_loans_async**](LoansApi.md#get_loans_async) | **GET** /api/v2/AccountingService/Loans | Gets all loans
[**get_loans_count_async**](LoansApi.md#get_loans_count_async) | **GET** /api/v2/AccountingService/Loans/Count | Counts loans
[**update_loan_application_async**](LoansApi.md#update_loan_application_async) | **PUT** /api/v2/AccountingService/Loans/Applications/{applicationId} | Updates a loan application
[**update_loan_async**](LoansApi.md#update_loan_async) | **PUT** /api/v2/AccountingService/Loans/{loanId} | Updates a loan



## create_loan_application_async

> models::EmptyEnvelope create_loan_application_async(tenant_id, loan_application_create_dto, api_version, x_api_version)
Creates a loan application

Creates a new loan application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loan_application_create_dto** | [**LoanApplicationCreateDto**](LoanApplicationCreateDto.md) |  | [required] |
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


## create_loan_async

> models::EmptyEnvelope create_loan_async(tenant_id, loan_create_dto, api_version, x_api_version)
Creates a new loan

Creates a new loan for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loan_create_dto** | [**LoanCreateDto**](LoanCreateDto.md) |  | [required] |
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


## delete_loan_application_async

> models::EmptyEnvelope delete_loan_application_async(tenant_id, application_id, api_version, x_api_version)
Deletes a loan application

Deletes the specified loan application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **uuid::Uuid** |  | [required] |
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


## delete_loan_async

> models::EmptyEnvelope delete_loan_async(tenant_id, loan_id, api_version, x_api_version)
Deletes a loan

Deletes the specified loan.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loan_id** | **uuid::Uuid** |  | [required] |
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


## get_loan_application_details_async

> models::LoanApplicationDtoEnvelope get_loan_application_details_async(tenant_id, application_id, api_version, x_api_version)
Gets a loan application by ID

Retrieves the details of a loan application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LoanApplicationDtoEnvelope**](LoanApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loan_applications_async

> models::LoanApplicationDtoIReadOnlyListEnvelope get_loan_applications_async(tenant_id, api_version, x_api_version)
Gets all loan applications

Retrieves all loan applications for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LoanApplicationDtoIReadOnlyListEnvelope**](LoanApplicationDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loan_applications_count_async

> models::Int32Envelope get_loan_applications_count_async(tenant_id, api_version, x_api_version)
Counts loan applications

Gets the count of loan applications for the current tenant.

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


## get_loan_details_async

> models::LoanDtoEnvelope get_loan_details_async(tenant_id, loan_id, api_version, x_api_version)
Gets a loan by ID

Retrieves the details of a loan using its unique ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loan_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LoanDtoEnvelope**](LoanDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loans_async

> models::LoanDtoIReadOnlyListEnvelope get_loans_async(tenant_id, api_version, x_api_version)
Gets all loans

Retrieves all loans for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::LoanDtoIReadOnlyListEnvelope**](LoanDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loans_count_async

> models::Int32Envelope get_loans_count_async(tenant_id, api_version, x_api_version)
Counts loans

Gets the count of loans for the current tenant.

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


## update_loan_application_async

> models::EmptyEnvelope update_loan_application_async(tenant_id, application_id, loan_application_update_dto, api_version, x_api_version)
Updates a loan application

Updates the specified loan application.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **uuid::Uuid** |  | [required] |
**loan_application_update_dto** | [**LoanApplicationUpdateDto**](LoanApplicationUpdateDto.md) |  | [required] |
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


## update_loan_async

> models::EmptyEnvelope update_loan_async(tenant_id, loan_id, loan_update_dto, api_version, x_api_version)
Updates a loan

Updates the specified loan.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loan_id** | **uuid::Uuid** |  | [required] |
**loan_update_dto** | [**LoanUpdateDto**](LoanUpdateDto.md) |  | [required] |
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

