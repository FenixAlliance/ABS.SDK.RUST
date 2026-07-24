# \SigningProfileGraphicalRepresentationsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#create_signing_profile_graphical_representation_async) | **POST** /api/v2/TrustService/SigningProfileGraphicalRepresentations | Create a new signature representation
[**delete_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#delete_signing_profile_graphical_representation_async) | **DELETE** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Delete a signature representation
[**get_signing_profile_graphical_representation_by_id_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representation_by_id_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Get signature representation by ID
[**get_signing_profile_graphical_representations_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representations_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations | Get all signature representations
[**get_signing_profile_graphical_representations_count_async**](SigningProfileGraphicalRepresentationsApi.md#get_signing_profile_graphical_representations_count_async) | **GET** /api/v2/TrustService/SigningProfileGraphicalRepresentations/Count | Get signature representations count
[**patch_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#patch_signing_profile_graphical_representation_async) | **PATCH** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Patch a signature representation
[**update_signing_profile_graphical_representation_async**](SigningProfileGraphicalRepresentationsApi.md#update_signing_profile_graphical_representation_async) | **PUT** /api/v2/TrustService/SigningProfileGraphicalRepresentations/{id} | Update a signature representation



## create_signing_profile_graphical_representation_async

> create_signing_profile_graphical_representation_async(tenant_id, api_version, x_api_version, signing_profile_graphical_representation_create_dto)
Create a new signature representation

Creates a new reusable signature representation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_graphical_representation_create_dto** | Option<[**SigningProfileGraphicalRepresentationCreateDto**](SigningProfileGraphicalRepresentationCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_signing_profile_graphical_representation_async

> delete_signing_profile_graphical_representation_async(tenant_id, id, api_version, x_api_version)
Delete a signature representation

Deletes a signature representation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## get_signing_profile_graphical_representation_by_id_async

> models::SigningProfileGraphicalRepresentationDto get_signing_profile_graphical_representation_by_id_async(tenant_id, id, api_version, x_api_version)
Get signature representation by ID

Retrieves a specific signature representation by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningProfileGraphicalRepresentationDto**](SigningProfileGraphicalRepresentationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_profile_graphical_representations_async

> models::SigningProfileGraphicalRepresentationDtoListEnvelope get_signing_profile_graphical_representations_async(tenant_id, api_version, x_api_version)
Get all signature representations

Retrieves all reusable signature representations for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SigningProfileGraphicalRepresentationDtoListEnvelope**](SigningProfileGraphicalRepresentationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_signing_profile_graphical_representations_count_async

> models::Int32Envelope get_signing_profile_graphical_representations_count_async(tenant_id, api_version, x_api_version)
Get signature representations count

Returns the count of signature representations for the specified tenant.

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


## patch_signing_profile_graphical_representation_async

> models::EmptyEnvelope patch_signing_profile_graphical_representation_async(tenant_id, id, api_version, x_api_version, operation)
Patch a signature representation

Patch a signature representation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
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


## update_signing_profile_graphical_representation_async

> update_signing_profile_graphical_representation_async(tenant_id, id, api_version, x_api_version, signing_profile_graphical_representation_update_dto)
Update a signature representation

Updates an existing signature representation for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**signing_profile_graphical_representation_update_dto** | Option<[**SigningProfileGraphicalRepresentationUpdateDto**](SigningProfileGraphicalRepresentationUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

