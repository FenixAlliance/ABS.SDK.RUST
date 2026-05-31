# \MarketingLeadsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_marketing_lead_async**](MarketingLeadsApi.md#create_marketing_lead_async) | **POST** /api/v2/MarketingService/MarketingLeads | Create a marketing lead
[**delete_marketing_lead_async**](MarketingLeadsApi.md#delete_marketing_lead_async) | **DELETE** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Delete a marketing lead
[**get_marketing_lead_details_async**](MarketingLeadsApi.md#get_marketing_lead_details_async) | **GET** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Get marketing lead by ID
[**get_marketing_leads_count_async**](MarketingLeadsApi.md#get_marketing_leads_count_async) | **GET** /api/v2/MarketingService/MarketingLeads/Count | Get marketing leads count
[**get_marketing_leads_o_data_async**](MarketingLeadsApi.md#get_marketing_leads_o_data_async) | **GET** /api/v2/MarketingService/MarketingLeads | Get marketing leads
[**update_marketing_lead_async**](MarketingLeadsApi.md#update_marketing_lead_async) | **PUT** /api/v2/MarketingService/MarketingLeads/{marketingLeadId} | Update a marketing lead



## create_marketing_lead_async

> models::EmptyEnvelope create_marketing_lead_async(tenant_id, marketing_lead_create_dto, api_version, x_api_version)
Create a marketing lead

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_lead_create_dto** | [**MarketingLeadCreateDto**](MarketingLeadCreateDto.md) |  | [required] |
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


## delete_marketing_lead_async

> models::EmptyEnvelope delete_marketing_lead_async(tenant_id, marketing_lead_id, api_version, x_api_version)
Delete a marketing lead

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_lead_id** | **uuid::Uuid** |  | [required] |
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


## get_marketing_lead_details_async

> models::MarketingLeadDtoEnvelope get_marketing_lead_details_async(tenant_id, marketing_lead_id, api_version, x_api_version)
Get marketing lead by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_lead_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingLeadDtoEnvelope**](MarketingLeadDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_leads_count_async

> models::Int32Envelope get_marketing_leads_count_async(tenant_id, api_version, x_api_version)
Get marketing leads count

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


## get_marketing_leads_o_data_async

> models::MarketingLeadDtoListEnvelope get_marketing_leads_o_data_async(tenant_id, api_version, x_api_version)
Get marketing leads

Retrieves a collection of marketing leads for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingLeadDtoListEnvelope**](MarketingLeadDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_marketing_lead_async

> models::EmptyEnvelope update_marketing_lead_async(tenant_id, marketing_lead_id, marketing_lead_update_dto, api_version, x_api_version)
Update a marketing lead

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_lead_id** | **uuid::Uuid** |  | [required] |
**marketing_lead_update_dto** | [**MarketingLeadUpdateDto**](MarketingLeadUpdateDto.md) |  | [required] |
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

