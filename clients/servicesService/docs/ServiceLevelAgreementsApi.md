# \ServiceLevelAgreementsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_level_agreement_async**](ServiceLevelAgreementsApi.md#create_service_level_agreement_async) | **POST** /api/v2/ServicesService/ServiceLevelAgreements | Create a service level agreement
[**delete_service_level_agreement_async**](ServiceLevelAgreementsApi.md#delete_service_level_agreement_async) | **DELETE** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Delete a service level agreement
[**get_service_level_agreement_by_id_async**](ServiceLevelAgreementsApi.md#get_service_level_agreement_by_id_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Get a service level agreement by ID
[**get_service_level_agreements_async**](ServiceLevelAgreementsApi.md#get_service_level_agreements_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements | Get all service level agreements
[**get_service_level_agreements_count_async**](ServiceLevelAgreementsApi.md#get_service_level_agreements_count_async) | **GET** /api/v2/ServicesService/ServiceLevelAgreements/Count | Get service level agreements count
[**patch_service_level_agreement_async**](ServiceLevelAgreementsApi.md#patch_service_level_agreement_async) | **PATCH** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Patch a service level agreement
[**update_service_level_agreement_async**](ServiceLevelAgreementsApi.md#update_service_level_agreement_async) | **PUT** /api/v2/ServicesService/ServiceLevelAgreements/{serviceLevelAgreementId} | Update a service level agreement



## create_service_level_agreement_async

> models::Envelope create_service_level_agreement_async(tenant_id, api_version, x_api_version, service_level_agreement_create_dto)
Create a service level agreement

Creates a new service level agreement for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_agreement_create_dto** | Option<[**ServiceLevelAgreementCreateDto**](ServiceLevelAgreementCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_service_level_agreement_async

> models::Envelope delete_service_level_agreement_async(tenant_id, service_level_agreement_id, api_version, x_api_version)
Delete a service level agreement

Deletes a service level agreement by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_level_agreement_id** | **uuid::Uuid** |  | [required] |
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


## get_service_level_agreement_by_id_async

> models::ServiceLevelAgreementDtoEnvelope get_service_level_agreement_by_id_async(tenant_id, service_level_agreement_id, api_version, x_api_version)
Get a service level agreement by ID

Retrieves a service level agreement by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_level_agreement_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceLevelAgreementDtoEnvelope**](ServiceLevelAgreementDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_level_agreements_async

> models::ServiceLevelAgreementDtoIReadOnlyListEnvelope get_service_level_agreements_async(tenant_id, api_version, x_api_version, service_level_agreement_dto_collection_query_parameters)
Get all service level agreements

Retrieves all service level agreements for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_agreement_dto_collection_query_parameters** | Option<[**ServiceLevelAgreementDtoCollectionQueryParameters**](ServiceLevelAgreementDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ServiceLevelAgreementDtoIReadOnlyListEnvelope**](ServiceLevelAgreementDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_level_agreements_count_async

> models::Int32Envelope get_service_level_agreements_count_async(tenant_id, api_version, x_api_version, service_level_agreement_dto_collection_query_parameters)
Get service level agreements count

Returns the count of service level agreements for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_agreement_dto_collection_query_parameters** | Option<[**ServiceLevelAgreementDtoCollectionQueryParameters**](ServiceLevelAgreementDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_service_level_agreement_async

> models::Envelope patch_service_level_agreement_async(tenant_id, service_level_agreement_id, api_version, x_api_version, patch_operation)
Patch a service level agreement

Partially updates an existing service level agreement using a JSON Patch document.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_level_agreement_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_service_level_agreement_async

> models::Envelope update_service_level_agreement_async(tenant_id, service_level_agreement_id, api_version, x_api_version, service_level_agreement_update_dto)
Update a service level agreement

Updates an existing service level agreement.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_level_agreement_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_level_agreement_update_dto** | Option<[**ServiceLevelAgreementUpdateDto**](ServiceLevelAgreementUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

