# \ExpenseTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_expense_type**](ExpenseTypesApi.md#create_expense_type) | **POST** /api/v2/AccountingService/ExpenseTypes | Create an expense type
[**delete_expense_type**](ExpenseTypesApi.md#delete_expense_type) | **DELETE** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Delete an expense type
[**get_expense_type**](ExpenseTypesApi.md#get_expense_type) | **GET** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Get an expense type by id
[**get_expense_types**](ExpenseTypesApi.md#get_expense_types) | **GET** /api/v2/AccountingService/ExpenseTypes | Get all expense types for a tenant
[**get_expense_types_count**](ExpenseTypesApi.md#get_expense_types_count) | **GET** /api/v2/AccountingService/ExpenseTypes/Count | Get the count of expense types for a tenant
[**update_expense_type**](ExpenseTypesApi.md#update_expense_type) | **PUT** /api/v2/AccountingService/ExpenseTypes/{expenseTypeId} | Update an expense type



## create_expense_type

> models::EmptyEnvelope create_expense_type(tenant_id, expense_type_create_dto, api_version, x_api_version)
Create an expense type

Creates a new expense type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_type_create_dto** | [**ExpenseTypeCreateDto**](ExpenseTypeCreateDto.md) |  | [required] |
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


## delete_expense_type

> models::EmptyEnvelope delete_expense_type(tenant_id, expense_type_id, api_version, x_api_version)
Delete an expense type

Deletes an expense type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_type_id** | **uuid::Uuid** |  | [required] |
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


## get_expense_type

> models::ExpenseTypeDtoEnvelope get_expense_type(tenant_id, expense_type_id, api_version, x_api_version)
Get an expense type by id

Retrieves an expense type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExpenseTypeDtoEnvelope**](ExpenseTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_expense_types

> models::ExpenseTypeDtoListEnvelope get_expense_types(tenant_id, api_version, x_api_version)
Get all expense types for a tenant

Retrieves all expense types for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExpenseTypeDtoListEnvelope**](ExpenseTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_expense_types_count

> models::Int32Envelope get_expense_types_count(tenant_id, api_version, x_api_version)
Get the count of expense types for a tenant

Retrieves the count of expense types for the specified tenant using OData query options.

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


## update_expense_type

> models::EmptyEnvelope update_expense_type(tenant_id, expense_type_id, expense_type_update_dto, api_version, x_api_version)
Update an expense type

Updates an existing expense type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**expense_type_id** | **uuid::Uuid** |  | [required] |
**expense_type_update_dto** | [**ExpenseTypeUpdateDto**](ExpenseTypeUpdateDto.md) |  | [required] |
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

