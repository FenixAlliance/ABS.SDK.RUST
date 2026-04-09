# \JobOffersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_job_offer_async**](JobOffersApi.md#create_job_offer_async) | **POST** /api/v2/HrmsService/JobOffers | Create a job offer
[**delete_job_offer_async**](JobOffersApi.md#delete_job_offer_async) | **DELETE** /api/v2/HrmsService/JobOffers/{jobOfferId} | Delete a job offer
[**get_job_offer_by_id_async**](JobOffersApi.md#get_job_offer_by_id_async) | **GET** /api/v2/HrmsService/JobOffers/{jobOfferId} | Get job offer by ID
[**get_job_offers_async**](JobOffersApi.md#get_job_offers_async) | **GET** /api/v2/HrmsService/JobOffers | Get job offers
[**get_job_offers_count_async**](JobOffersApi.md#get_job_offers_count_async) | **GET** /api/v2/HrmsService/JobOffers/Count | Count job offers
[**update_job_offer_async**](JobOffersApi.md#update_job_offer_async) | **PUT** /api/v2/HrmsService/JobOffers/{jobOfferId} | Update a job offer



## create_job_offer_async

> models::EmptyEnvelope create_job_offer_async(tenant_id, api_version, x_api_version, job_offer_create_dto)
Create a job offer

Creates a new job offer for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**job_offer_create_dto** | Option<[**JobOfferCreateDto**](JobOfferCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_job_offer_async

> models::EmptyEnvelope delete_job_offer_async(tenant_id, job_offer_id, api_version, x_api_version)
Delete a job offer

Deletes a job offer for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_id** | **uuid::Uuid** |  | [required] |
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


## get_job_offer_by_id_async

> models::JobOfferDtoEnvelope get_job_offer_by_id_async(tenant_id, job_offer_id, api_version, x_api_version)
Get job offer by ID

Retrieves a specific job offer by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobOfferDtoEnvelope**](JobOfferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_offers_async

> models::JobOfferDtoListEnvelope get_job_offers_async(tenant_id, api_version, x_api_version)
Get job offers

Retrieves job offers for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::JobOfferDtoListEnvelope**](JobOfferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_job_offers_count_async

> models::Int32Envelope get_job_offers_count_async(tenant_id, api_version, x_api_version)
Count job offers

Counts job offers for the specified tenant.

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


## update_job_offer_async

> models::EmptyEnvelope update_job_offer_async(tenant_id, job_offer_id, api_version, x_api_version, body)
Update a job offer

Updates an existing job offer for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**job_offer_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**body** | Option<**serde_json::Value**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

