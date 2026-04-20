# \SocialGroupsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_social_groups_async**](SocialGroupsApi.md#count_social_groups_async) | **GET** /api/v2/SocialService/SocialGroups/Count | Count social groups
[**create_social_group_async**](SocialGroupsApi.md#create_social_group_async) | **POST** /api/v2/SocialService/SocialGroups | Create a social group
[**delete_social_group_async**](SocialGroupsApi.md#delete_social_group_async) | **DELETE** /api/v2/SocialService/SocialGroups/{socialGroupId} | Delete a social group
[**get_social_group_by_id_async**](SocialGroupsApi.md#get_social_group_by_id_async) | **GET** /api/v2/SocialService/SocialGroups/{socialGroupId} | Get social group by ID
[**get_social_groups_async**](SocialGroupsApi.md#get_social_groups_async) | **GET** /api/v2/SocialService/SocialGroups | Get social groups
[**update_social_group_async**](SocialGroupsApi.md#update_social_group_async) | **PUT** /api/v2/SocialService/SocialGroups/{socialGroupId} | Update a social group



## count_social_groups_async

> models::Int32Envelope count_social_groups_async(tenant_id, api_version, x_api_version)
Count social groups

Counts all social groups for the specified tenant.

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


## create_social_group_async

> models::EmptyEnvelope create_social_group_async(tenant_id, api_version, x_api_version, social_group_create_dto)
Create a social group

Creates a new social group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_group_create_dto** | Option<[**SocialGroupCreateDto**](SocialGroupCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_social_group_async

> models::EmptyEnvelope delete_social_group_async(tenant_id, social_group_id, api_version, x_api_version)
Delete a social group

Deletes a social group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**social_group_id** | **uuid::Uuid** |  | [required] |
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


## get_social_group_by_id_async

> models::SocialGroupDtoEnvelope get_social_group_by_id_async(tenant_id, social_group_id, api_version, x_api_version)
Get social group by ID

Retrieves a specific social group by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**social_group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialGroupDtoEnvelope**](SocialGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_social_groups_async

> models::SocialGroupDtoListEnvelope get_social_groups_async(tenant_id, api_version, x_api_version)
Get social groups

Retrieves all social groups for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialGroupDtoListEnvelope**](SocialGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_social_group_async

> models::EmptyEnvelope update_social_group_async(tenant_id, social_group_id, api_version, x_api_version, social_group_update_dto)
Update a social group

Updates an existing social group for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**social_group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**social_group_update_dto** | Option<[**SocialGroupUpdateDto**](SocialGroupUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

