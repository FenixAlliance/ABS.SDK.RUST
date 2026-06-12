# \NonFungibleTokensApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_non_fungible_token_async**](NonFungibleTokensApi.md#create_non_fungible_token_async) | **POST** /api/v2/BlockchainsService/NonFungibleTokens | Create a new NFT
[**delete_non_fungible_token_async**](NonFungibleTokensApi.md#delete_non_fungible_token_async) | **DELETE** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Delete an NFT
[**get_non_fungible_token_by_id_async**](NonFungibleTokensApi.md#get_non_fungible_token_by_id_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Get NFT by ID
[**get_non_fungible_tokens_async**](NonFungibleTokensApi.md#get_non_fungible_tokens_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens | Get all non-fungible tokens
[**get_non_fungible_tokens_count_async**](NonFungibleTokensApi.md#get_non_fungible_tokens_count_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens/Count | Get NFTs count
[**patch_non_fungible_token_async**](NonFungibleTokensApi.md#patch_non_fungible_token_async) | **PATCH** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Patch a non-fungible token
[**update_non_fungible_token_async**](NonFungibleTokensApi.md#update_non_fungible_token_async) | **PUT** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Update an NFT



## create_non_fungible_token_async

> create_non_fungible_token_async(tenant_id, api_version, x_api_version, non_fungible_token_create_dto)
Create a new NFT

Creates a new non-fungible token for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**non_fungible_token_create_dto** | Option<[**NonFungibleTokenCreateDto**](NonFungibleTokenCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_non_fungible_token_async

> delete_non_fungible_token_async(tenant_id, id, api_version, x_api_version)
Delete an NFT

Deletes a non-fungible token for the specified tenant.

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


## get_non_fungible_token_by_id_async

> models::NonFungibleTokenDto get_non_fungible_token_by_id_async(tenant_id, id, api_version, x_api_version)
Get NFT by ID

Retrieves a specific non-fungible token by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NonFungibleTokenDto**](NonFungibleTokenDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_non_fungible_tokens_async

> models::NonFungibleTokenDtoListEnvelope get_non_fungible_tokens_async(tenant_id, o_data_query_options, api_version, x_api_version)
Get all non-fungible tokens

Retrieves all NFTs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**o_data_query_options** | Option<[**NonFungibleTokenDtoODataQueryOptions**](.md)> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NonFungibleTokenDtoListEnvelope**](NonFungibleTokenDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_non_fungible_tokens_count_async

> models::Int32Envelope get_non_fungible_tokens_count_async(tenant_id, o_data_query_options, api_version, x_api_version)
Get NFTs count

Returns the count of NFTs for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**o_data_query_options** | Option<[**NonFungibleTokenDtoODataQueryOptions**](.md)> |  |  |
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


## patch_non_fungible_token_async

> models::EmptyEnvelope patch_non_fungible_token_async(tenant_id, id, api_version, x_api_version, operation)
Patch a non-fungible token

Patch a non-fungible token

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


## update_non_fungible_token_async

> update_non_fungible_token_async(tenant_id, id, api_version, x_api_version, non_fungible_token_update_dto)
Update an NFT

Updates an existing non-fungible token for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**non_fungible_token_update_dto** | Option<[**NonFungibleTokenUpdateDto**](NonFungibleTokenUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

