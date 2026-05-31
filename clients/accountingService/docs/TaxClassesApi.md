# \TaxClassesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tax_class**](TaxClassesApi.md#create_tax_class) | **POST** /api/v2/AccountingService/TaxClasses | Create a tax class
[**delete_tax_class**](TaxClassesApi.md#delete_tax_class) | **DELETE** /api/v2/AccountingService/TaxClasses/{id} | Delete a tax class
[**get_tax_class**](TaxClassesApi.md#get_tax_class) | **GET** /api/v2/AccountingService/TaxClasses/{id} | Get tax class by ID
[**get_tax_classes**](TaxClassesApi.md#get_tax_classes) | **GET** /api/v2/AccountingService/TaxClasses | Get all tax classes for a tenant
[**get_tax_classes_count**](TaxClassesApi.md#get_tax_classes_count) | **GET** /api/v2/AccountingService/TaxClasses/Count | Get tax classes count
[**update_tax_class**](TaxClassesApi.md#update_tax_class) | **PUT** /api/v2/AccountingService/TaxClasses/{id} | Update a tax class



## create_tax_class

> models::EmptyEnvelope create_tax_class(tenant_id, api_version, x_api_version, tax_class_create_dto)
Create a tax class

Creates a new tax class for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_class_create_dto** | Option<[**TaxClassCreateDto**](TaxClassCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tax_class

> models::EmptyEnvelope delete_tax_class(tenant_id, id, api_version, x_api_version)
Delete a tax class

Deletes a tax class identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_tax_class

> models::TaxClassDtoEnvelope get_tax_class(tenant_id, id, api_version, x_api_version)
Get tax class by ID

Retrieves a specific tax class by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxClassDtoEnvelope**](TaxClassDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_classes

> models::TaxClassDtoListEnvelope get_tax_classes(tenant_id, api_version, x_api_version)
Get all tax classes for a tenant

Retrieves all tax classes for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TaxClassDtoListEnvelope**](TaxClassDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tax_classes_count

> models::Int32Envelope get_tax_classes_count(tenant_id, api_version, x_api_version)
Get tax classes count

Returns the count of tax classes for the specified tenant.

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


## update_tax_class

> models::EmptyEnvelope update_tax_class(tenant_id, id, api_version, x_api_version, tax_class_update_dto)
Update a tax class

Updates an existing tax class identified by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tax_class_update_dto** | Option<[**TaxClassUpdateDto**](TaxClassUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

