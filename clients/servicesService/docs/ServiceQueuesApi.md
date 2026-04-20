# \ServiceQueuesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_service_queue_async**](ServiceQueuesApi.md#create_service_queue_async) | **POST** /api/v2/ServicesService/ServiceQueues | Create a service queue
[**delete_service_queue_async**](ServiceQueuesApi.md#delete_service_queue_async) | **DELETE** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Delete a service queue
[**get_service_queue_by_id_async**](ServiceQueuesApi.md#get_service_queue_by_id_async) | **GET** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Get a service queue by ID
[**get_service_queues_async**](ServiceQueuesApi.md#get_service_queues_async) | **GET** /api/v2/ServicesService/ServiceQueues | Get all service queues
[**get_service_queues_count_async**](ServiceQueuesApi.md#get_service_queues_count_async) | **GET** /api/v2/ServicesService/ServiceQueues/Count | Get service queues count
[**update_service_queue_async**](ServiceQueuesApi.md#update_service_queue_async) | **PUT** /api/v2/ServicesService/ServiceQueues/{serviceQueueId} | Update a service queue



## create_service_queue_async

> models::Envelope create_service_queue_async(tenant_id, api_version, x_api_version, service_queue_create_dto)
Create a service queue

Creates a new service queue for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_queue_create_dto** | Option<[**ServiceQueueCreateDto**](ServiceQueueCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_service_queue_async

> models::Envelope delete_service_queue_async(tenant_id, service_queue_id, api_version, x_api_version)
Delete a service queue

Deletes a service queue by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_queue_id** | **uuid::Uuid** |  | [required] |
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


## get_service_queue_by_id_async

> models::ServiceQueueDtoEnvelope get_service_queue_by_id_async(tenant_id, service_queue_id, api_version, x_api_version)
Get a service queue by ID

Retrieves a service queue by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_queue_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceQueueDtoEnvelope**](ServiceQueueDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_queues_async

> models::ServiceQueueDtoIReadOnlyListEnvelope get_service_queues_async(tenant_id, api_version, x_api_version)
Get all service queues

Retrieves all service queues for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ServiceQueueDtoIReadOnlyListEnvelope**](ServiceQueueDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_service_queues_count_async

> models::Int32Envelope get_service_queues_count_async(tenant_id, api_version, x_api_version)
Get service queues count

Returns the count of service queues for the specified tenant.

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


## update_service_queue_async

> models::Envelope update_service_queue_async(tenant_id, service_queue_id, api_version, x_api_version, service_queue_update_dto)
Update a service queue

Updates an existing service queue.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**service_queue_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**service_queue_update_dto** | Option<[**ServiceQueueUpdateDto**](ServiceQueueUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

