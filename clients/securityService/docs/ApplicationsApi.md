# \ApplicationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_business_application_async**](ApplicationsApi.md#create_business_application_async) | **POST** /api/v2/SecurityService/Applications | Create a new business application
[**delete_business_application_async**](ApplicationsApi.md#delete_business_application_async) | **DELETE** /api/v2/SecurityService/Applications/{applicationId} | Delete a business application
[**get_business_application_by_id_async**](ApplicationsApi.md#get_business_application_by_id_async) | **GET** /api/v2/SecurityService/Applications/{applicationId} | Get business application by ID
[**get_business_applications_async**](ApplicationsApi.md#get_business_applications_async) | **GET** /api/v2/SecurityService/Applications | Get all business applications
[**get_business_applications_count_async**](ApplicationsApi.md#get_business_applications_count_async) | **GET** /api/v2/SecurityService/Applications/Count | Get business applications count
[**update_business_application_async**](ApplicationsApi.md#update_business_application_async) | **PUT** /api/v2/SecurityService/Applications/{applicationId} | Update an existing business application



## create_business_application_async

> models::EmptyEnvelope create_business_application_async(tenant_id, business_application_create_dto, api_version, x_api_version)
Create a new business application

Creates a new business application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**business_application_create_dto** | [**BusinessApplicationCreateDto**](BusinessApplicationCreateDto.md) |  | [required] |
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


## delete_business_application_async

> models::EmptyEnvelope delete_business_application_async(tenant_id, application_id, api_version, x_api_version)
Delete a business application

Deletes an existing business application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
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


## get_business_application_by_id_async

> models::BusinessApplicationDtoEnvelope get_business_application_by_id_async(tenant_id, application_id, api_version, x_api_version)
Get business application by ID

Retrieves a specific business application by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessApplicationDtoEnvelope**](BusinessApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_applications_async

> models::BusinessApplicationDtoListEnvelope get_business_applications_async(tenant_id, api_version, x_api_version)
Get all business applications

Retrieves all business applications for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BusinessApplicationDtoListEnvelope**](BusinessApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_applications_count_async

> models::Int32Envelope get_business_applications_count_async(tenant_id, api_version, x_api_version)
Get business applications count

Retrieves the count of business applications for the specified tenant.

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


## update_business_application_async

> models::EmptyEnvelope update_business_application_async(tenant_id, application_id, business_application_update_dto, api_version, x_api_version)
Update an existing business application

Updates an existing business application for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**application_id** | **String** |  | [required] |
**business_application_update_dto** | [**BusinessApplicationUpdateDto**](BusinessApplicationUpdateDto.md) |  | [required] |
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

