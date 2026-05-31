# \GigsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_gig_async**](GigsApi.md#create_gig_async) | **POST** /api/v2/HrmsService/Gigs | Create a gig
[**delete_gig_async**](GigsApi.md#delete_gig_async) | **DELETE** /api/v2/HrmsService/Gigs/{gigId} | Delete a gig
[**get_gig_by_id_async**](GigsApi.md#get_gig_by_id_async) | **GET** /api/v2/HrmsService/Gigs/{gigId} | Get gig by ID
[**get_gigs_async**](GigsApi.md#get_gigs_async) | **GET** /api/v2/HrmsService/Gigs | Get gigs
[**get_gigs_count_async**](GigsApi.md#get_gigs_count_async) | **GET** /api/v2/HrmsService/Gigs/Count | Count gigs
[**update_gig_async**](GigsApi.md#update_gig_async) | **PUT** /api/v2/HrmsService/Gigs/{gigId} | Update a gig



## create_gig_async

> models::EmptyEnvelope create_gig_async(tenant_id, api_version, x_api_version, gig_create_dto)
Create a gig

Creates a new gig for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**gig_create_dto** | Option<[**GigCreateDto**](GigCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_gig_async

> models::EmptyEnvelope delete_gig_async(tenant_id, gig_id, api_version, x_api_version)
Delete a gig

Deletes a gig for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_id** | **uuid::Uuid** |  | [required] |
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


## get_gig_by_id_async

> models::GigDtoEnvelope get_gig_by_id_async(tenant_id, gig_id, api_version, x_api_version)
Get gig by ID

Retrieves a specific gig by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GigDtoEnvelope**](GigDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_gigs_async

> models::GigDtoListEnvelope get_gigs_async(tenant_id, api_version, x_api_version)
Get gigs

Retrieves gigs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GigDtoListEnvelope**](GigDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_gigs_count_async

> models::Int32Envelope get_gigs_count_async(tenant_id, api_version, x_api_version)
Count gigs

Counts gigs for the specified tenant.

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


## update_gig_async

> models::EmptyEnvelope update_gig_async(tenant_id, gig_id, api_version, x_api_version, gig_update_dto)
Update a gig

Updates an existing gig for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**gig_update_dto** | Option<[**GigUpdateDto**](GigUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

