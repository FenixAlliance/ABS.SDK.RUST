# \GigApplicationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accept_gig_application_async**](GigApplicationsApi.md#accept_gig_application_async) | **POST** /api/v2/HrmsService/GigApplications/{gigApplicationId}/Accept | Accept a gig application
[**create_gig_application_async**](GigApplicationsApi.md#create_gig_application_async) | **POST** /api/v2/HrmsService/GigApplications | Create a gig application
[**delete_gig_application_async**](GigApplicationsApi.md#delete_gig_application_async) | **DELETE** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Delete a gig application
[**get_gig_application_by_id_async**](GigApplicationsApi.md#get_gig_application_by_id_async) | **GET** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Get gig application by ID
[**get_gig_applications_async**](GigApplicationsApi.md#get_gig_applications_async) | **GET** /api/v2/HrmsService/GigApplications | Get gig applications
[**get_gig_applications_count_async**](GigApplicationsApi.md#get_gig_applications_count_async) | **GET** /api/v2/HrmsService/GigApplications/Count | Count gig applications
[**patch_gig_application_async**](GigApplicationsApi.md#patch_gig_application_async) | **PATCH** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Patch a gig application
[**update_gig_application_async**](GigApplicationsApi.md#update_gig_application_async) | **PUT** /api/v2/HrmsService/GigApplications/{gigApplicationId} | Update a gig application



## accept_gig_application_async

> models::EmptyEnvelope accept_gig_application_async(tenant_id, gig_application_id, api_version, x_api_version)
Accept a gig application

Accepts the candidate's gig proposal, forming an engagement (raises GigApplicationAccepted). A proposal cannot be accepted twice.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_application_id** | **uuid::Uuid** |  | [required] |
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


## create_gig_application_async

> models::EmptyEnvelope create_gig_application_async(tenant_id, api_version, x_api_version, gig_application_create_dto)
Create a gig application

Records a candidate's proposal against one of the tenant's gigs. The targeted gig must belong to the tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**gig_application_create_dto** | Option<[**GigApplicationCreateDto**](GigApplicationCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_gig_application_async

> models::EmptyEnvelope delete_gig_application_async(tenant_id, gig_application_id, api_version, x_api_version)
Delete a gig application

Removes a proposal submitted against one of the tenant's gigs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_application_id** | **uuid::Uuid** |  | [required] |
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


## get_gig_application_by_id_async

> models::GigApplicationDtoEnvelope get_gig_application_by_id_async(tenant_id, gig_application_id, api_version, x_api_version)
Get gig application by ID

Retrieves a specific proposal submitted against one of the tenant's gigs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GigApplicationDtoEnvelope**](GigApplicationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_gig_applications_async

> models::GigApplicationDtoListEnvelope get_gig_applications_async(tenant_id, api_version, x_api_version)
Get gig applications

Retrieves proposals submitted against the tenant's gigs. Filter with `$filter=GigId eq '...'` or `JobApplicantProfileId eq '...'`.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::GigApplicationDtoListEnvelope**](GigApplicationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_gig_applications_count_async

> models::Int32Envelope get_gig_applications_count_async(tenant_id, api_version, x_api_version)
Count gig applications

Counts proposals submitted against the tenant's gigs.

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


## patch_gig_application_async

> models::EmptyEnvelope patch_gig_application_async(tenant_id, gig_application_id, api_version, x_api_version, operation)
Patch a gig application

Partially updates an existing proposal submitted against one of the tenant's gigs.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_gig_application_async

> models::EmptyEnvelope update_gig_application_async(tenant_id, gig_application_id, api_version, x_api_version, gig_application_update_dto)
Update a gig application

Updates an existing proposal submitted against one of the tenant's gigs (e.g. accept it).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**gig_application_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**gig_application_update_dto** | Option<[**GigApplicationUpdateDto**](GigApplicationUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

