# \MarketingCampaignsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_marketing_campaign_async**](MarketingCampaignsApi.md#create_marketing_campaign_async) | **POST** /api/v2/MarketingService/MarketingCampaigns | Create a marketing campaign
[**delete_marketing_campaign_async**](MarketingCampaignsApi.md#delete_marketing_campaign_async) | **DELETE** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Delete a marketing campaign
[**get_marketing_campaign_details_async**](MarketingCampaignsApi.md#get_marketing_campaign_details_async) | **GET** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Get marketing campaign by ID
[**get_marketing_campaign_o_data_async**](MarketingCampaignsApi.md#get_marketing_campaign_o_data_async) | **GET** /api/v2/MarketingService/MarketingCampaigns | Get marketing campaigns
[**get_marketing_campaigns_count_async**](MarketingCampaignsApi.md#get_marketing_campaigns_count_async) | **GET** /api/v2/MarketingService/MarketingCampaigns/Count | Get marketing campaigns count
[**update_marketing_campaign_async**](MarketingCampaignsApi.md#update_marketing_campaign_async) | **PUT** /api/v2/MarketingService/MarketingCampaigns/{marketingcampaignId} | Update a marketing campaign



## create_marketing_campaign_async

> models::EmptyEnvelope create_marketing_campaign_async(tenant_id, marketing_campaign_create_dto, api_version, x_api_version)
Create a marketing campaign

Creates a new marketing campaign for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketing_campaign_create_dto** | [**MarketingCampaignCreateDto**](MarketingCampaignCreateDto.md) |  | [required] |
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


## delete_marketing_campaign_async

> models::EmptyEnvelope delete_marketing_campaign_async(tenant_id, marketingcampaign_id, api_version, x_api_version)
Delete a marketing campaign

Deletes a marketing campaign by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketingcampaign_id** | **uuid::Uuid** |  | [required] |
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


## get_marketing_campaign_details_async

> models::MarketingCampaignDtoEnvelope get_marketing_campaign_details_async(tenant_id, marketingcampaign_id, api_version, x_api_version)
Get marketing campaign by ID

Retrieves the details of a specific marketing campaign by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketingcampaign_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MarketingCampaignDtoEnvelope**](MarketingCampaignDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_campaign_o_data_async

> get_marketing_campaign_o_data_async(tenant_id, api_version, x_api_version)
Get marketing campaigns

Retrieves a collection of marketing campaigns for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_marketing_campaigns_count_async

> models::Int32Envelope get_marketing_campaigns_count_async(tenant_id, api_version, x_api_version)
Get marketing campaigns count

Returns the count of marketing campaigns for the specified tenant using OData query options.

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


## update_marketing_campaign_async

> models::EmptyEnvelope update_marketing_campaign_async(tenant_id, marketingcampaign_id, marketing_campaign_update_dto, api_version, x_api_version)
Update a marketing campaign

Updates an existing marketing campaign by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**marketingcampaign_id** | **uuid::Uuid** |  | [required] |
**marketing_campaign_update_dto** | [**MarketingCampaignUpdateDto**](MarketingCampaignUpdateDto.md) |  | [required] |
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

