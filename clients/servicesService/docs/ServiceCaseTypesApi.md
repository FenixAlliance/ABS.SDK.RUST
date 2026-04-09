# \ServiceCaseTypesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_case_type_async**](ServiceCaseTypesApi.md#create_service_case_type_async) | **POST** /api/v2/ServicesService/ServiceCaseTypes | Create a service case type
[**delete_service_case_type_async**](ServiceCaseTypesApi.md#delete_service_case_type_async) | **DELETE** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Delete a service case type
[**get_service_case_type_by_id_async**](ServiceCaseTypesApi.md#get_service_case_type_by_id_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Get a service case type by ID
[**get_service_case_types_async**](ServiceCaseTypesApi.md#get_service_case_types_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes | Get all service case types
[**get_service_case_types_count_async**](ServiceCaseTypesApi.md#get_service_case_types_count_async) | **GET** /api/v2/ServicesService/ServiceCaseTypes/Count | Get service case types count
[**update_service_case_type_async**](ServiceCaseTypesApi.md#update_service_case_type_async) | **PUT** /api/v2/ServicesService/ServiceCaseTypes/{serviceCaseTypeId} | Update a service case type



## create_service_case_type_async

> models::Envelope create_service_case_type_async(tenant_id, api_version, x_api_version, service_case_type_create_dto)
Create a service case type

Creates a new service case type for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_case_type_create_dto** | Option<[**ServiceCaseTypeCreateDto**](ServiceCaseTypeCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_service_case_type_async

> models::Envelope delete_service_case_type_async(tenant_id, service_case_type_id, api_version, x_api_version)
Delete a service case type

Deletes a service case type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_type_id** | **uuid::Uuid** |  | [required] |
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


## get_service_case_type_by_id_async

> models::ServiceCaseTypeDtoEnvelope get_service_case_type_by_id_async(tenant_id, service_case_type_id, api_version, x_api_version)
Get a service case type by ID

Retrieves a service case type by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceCaseTypeDtoEnvelope**](ServiceCaseTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_case_types_async

> models::ServiceCaseTypeDtoIReadOnlyListEnvelope get_service_case_types_async(tenant_id, api_version, x_api_version)
Get all service case types

Retrieves all service case types for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceCaseTypeDtoIReadOnlyListEnvelope**](ServiceCaseTypeDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_case_types_count_async

> models::Int32Envelope get_service_case_types_count_async(tenant_id, api_version, x_api_version)
Get service case types count

Returns the count of service case types for the specified tenant.

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


## update_service_case_type_async

> models::Envelope update_service_case_type_async(tenant_id, service_case_type_id, api_version, x_api_version, service_case_type_update_dto)
Update a service case type

Updates an existing service case type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_case_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_case_type_update_dto** | Option<[**ServiceCaseTypeUpdateDto**](ServiceCaseTypeUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

