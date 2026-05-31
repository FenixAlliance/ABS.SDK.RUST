# \ItemRetainSamplesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_retain_sample_async**](ItemRetainSamplesApi.md#create_item_retain_sample_async) | **POST** /api/v2/LogisticsService/ItemRetainSamples | Create an item retain sample
[**delete_item_retain_sample_async**](ItemRetainSamplesApi.md#delete_item_retain_sample_async) | **DELETE** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Delete an item retain sample
[**get_item_retain_sample_by_id_async**](ItemRetainSamplesApi.md#get_item_retain_sample_by_id_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Get item retain sample by ID
[**get_item_retain_samples_async**](ItemRetainSamplesApi.md#get_item_retain_samples_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples | Get all item retain samples
[**get_item_retain_samples_count_async**](ItemRetainSamplesApi.md#get_item_retain_samples_count_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/Count | Get item retain samples count
[**update_item_retain_sample_async**](ItemRetainSamplesApi.md#update_item_retain_sample_async) | **PUT** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Update an item retain sample



## create_item_retain_sample_async

> models::EmptyEnvelope create_item_retain_sample_async(tenant_id, api_version, x_api_version, item_retain_sample_create_dto)
Create an item retain sample

Creates a new item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_retain_sample_create_dto** | Option<[**ItemRetainSampleCreateDto**](ItemRetainSampleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_retain_sample_async

> models::EmptyEnvelope delete_item_retain_sample_async(tenant_id, retain_sample_id, api_version, x_api_version)
Delete an item retain sample

Deletes an item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
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


## get_item_retain_sample_by_id_async

> models::ItemRetainSampleDtoEnvelope get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, api_version, x_api_version)
Get item retain sample by ID

Retrieves a specific item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRetainSampleDtoEnvelope**](ItemRetainSampleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_retain_samples_async

> models::ItemRetainSampleDtoListEnvelope get_item_retain_samples_async(tenant_id, api_version, x_api_version)
Get all item retain samples

Retrieves all item retain samples for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRetainSampleDtoListEnvelope**](ItemRetainSampleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_retain_samples_count_async

> models::Int32Envelope get_item_retain_samples_count_async(tenant_id, api_version, x_api_version)
Get item retain samples count

Returns the count of item retain samples.

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


## update_item_retain_sample_async

> models::EmptyEnvelope update_item_retain_sample_async(tenant_id, retain_sample_id, api_version, x_api_version, item_retain_sample_update_dto)
Update an item retain sample

Updates an existing item retain sample.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**retain_sample_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_retain_sample_update_dto** | Option<[**ItemRetainSampleUpdateDto**](ItemRetainSampleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

