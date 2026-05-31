# \ServiceCasesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_case_async**](ServiceCasesApi.md#create_service_case_async) | **POST** /api/v2/ServicesService/ServiceCases | Create a service case
[**delete_service_case_async**](ServiceCasesApi.md#delete_service_case_async) | **DELETE** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Delete a service case
[**get_service_case_by_id_async**](ServiceCasesApi.md#get_service_case_by_id_async) | **GET** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Get a service case by ID
[**get_service_cases_async**](ServiceCasesApi.md#get_service_cases_async) | **GET** /api/v2/ServicesService/ServiceCases | Get all service cases
[**get_service_cases_count_async**](ServiceCasesApi.md#get_service_cases_count_async) | **GET** /api/v2/ServicesService/ServiceCases/Count | Get service cases count
[**update_service_case_async**](ServiceCasesApi.md#update_service_case_async) | **PUT** /api/v2/ServicesService/ServiceCases/{serviceCaseId} | Update a service case



## create_service_case_async

> models::Envelope create_service_case_async(tenant_id, api_version, x_api_version, service_case_create_dto)
Create a service case

Creates a new service case for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_case_create_dto** | Option<[**ServiceCaseCreateDto**](ServiceCaseCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_service_case_async

> models::Envelope delete_service_case_async(tenant_id, service_case_id, api_version, x_api_version)
Delete a service case

Deletes a service case by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_case_by_id_async

> models::ServiceCaseDtoEnvelope get_service_case_by_id_async(tenant_id, service_case_id, api_version, x_api_version)
Get a service case by ID

Retrieves a service case by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceCaseDtoEnvelope**](ServiceCaseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_cases_async

> models::ServiceCaseDtoIReadOnlyListEnvelope get_service_cases_async(tenant_id, api_version, x_api_version)
Get all service cases

Retrieves all service cases for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceCaseDtoIReadOnlyListEnvelope**](ServiceCaseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_cases_count_async

> models::Int32Envelope get_service_cases_count_async(tenant_id, api_version, x_api_version)
Get service cases count

Returns the count of service cases for the specified tenant.

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


## update_service_case_async

> models::Envelope update_service_case_async(tenant_id, service_case_id, api_version, x_api_version, service_case_update_dto)
Update a service case

Updates an existing service case.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_case_update_dto** | Option<[**ServiceCaseUpdateDto**](ServiceCaseUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

