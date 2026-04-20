# \SegmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_segment**](SegmentsApi.md#create_tenant_segment) | **POST** /api/v2/TenantsService/Segments | Create a new tenant segment
[**delete_tenant_segment**](SegmentsApi.md#delete_tenant_segment) | **DELETE** /api/v2/TenantsService/Segments/{tenantSegmentId} | Delete a tenant segment
[**get_tenant_segment_by_id**](SegmentsApi.md#get_tenant_segment_by_id) | **GET** /api/v2/TenantsService/Segments/{tenantSegmentId} | Retrieve a single tenant segment by its ID
[**get_tenant_segments**](SegmentsApi.md#get_tenant_segments) | **GET** /api/v2/TenantsService/Segments | Retrieve a list of tenant segments
[**get_tenant_segments_count**](SegmentsApi.md#get_tenant_segments_count) | **GET** /api/v2/TenantsService/Segments/Count | Get the count of tenant segments
[**update_tenant_segment**](SegmentsApi.md#update_tenant_segment) | **PUT** /api/v2/TenantsService/Segments/{tenantSegmentId} | Update a tenant segment



## create_tenant_segment

> models::EmptyEnvelope create_tenant_segment(tenant_id, api_version, x_api_version, tenant_segment_create_dto)
Create a new tenant segment

Create a new tenant segment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_segment_create_dto** | Option<[**TenantSegmentCreateDto**](TenantSegmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_segment

> models::EmptyEnvelope delete_tenant_segment(tenant_id, tenant_segment_id, api_version, x_api_version)
Delete a tenant segment

Delete a tenant segment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_segment_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_segment_by_id

> models::TenantSegmentDtoEnvelope get_tenant_segment_by_id(tenant_id, tenant_segment_id, api_version, x_api_version)
Retrieve a single tenant segment by its ID

Retrieve a single tenant segment by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_segment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantSegmentDtoEnvelope**](TenantSegmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_segments

> models::TenantSegmentDtoListEnvelope get_tenant_segments(tenant_id, api_version, x_api_version)
Retrieve a list of tenant segments

Retrieve a list of tenant segments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantSegmentDtoListEnvelope**](TenantSegmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_segments_count

> models::Int32Envelope get_tenant_segments_count(tenant_id, api_version, x_api_version)
Get the count of tenant segments

Get the count of tenant segments

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


## update_tenant_segment

> models::EmptyEnvelope update_tenant_segment(tenant_id, tenant_segment_id, api_version, x_api_version, tenant_segment_update_dto)
Update a tenant segment

Update a tenant segment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_segment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_segment_update_dto** | Option<[**TenantSegmentUpdateDto**](TenantSegmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

