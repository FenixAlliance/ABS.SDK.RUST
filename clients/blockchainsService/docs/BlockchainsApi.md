# \BlockchainsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_blockchain_async**](BlockchainsApi.md#create_blockchain_async) | **POST** /api/v2/BlockchainsService/Blockchains | Create a new blockchain
[**create_blockchain_block_async**](BlockchainsApi.md#create_blockchain_block_async) | **POST** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks | Add a block to a blockchain
[**delete_blockchain_async**](BlockchainsApi.md#delete_blockchain_async) | **DELETE** /api/v2/BlockchainsService/Blockchains/{id} | Delete a blockchain
[**delete_blockchain_block_async**](BlockchainsApi.md#delete_blockchain_block_async) | **DELETE** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Delete a blockchain block
[**get_blockchain_block_by_id_async**](BlockchainsApi.md#get_blockchain_block_by_id_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Get a specific block
[**get_blockchain_blocks_async**](BlockchainsApi.md#get_blockchain_blocks_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks | Get blocks for a blockchain
[**get_blockchain_blocks_count_async**](BlockchainsApi.md#get_blockchain_blocks_count_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/Count | Get block count for a blockchain
[**get_blockchain_by_id_async**](BlockchainsApi.md#get_blockchain_by_id_async) | **GET** /api/v2/BlockchainsService/Blockchains/{id} | Get blockchain by ID
[**get_blockchains_async**](BlockchainsApi.md#get_blockchains_async) | **GET** /api/v2/BlockchainsService/Blockchains | Get all blockchains
[**get_blockchains_count_async**](BlockchainsApi.md#get_blockchains_count_async) | **GET** /api/v2/BlockchainsService/Blockchains/Count | Get blockchains count
[**patch_blockchain_async**](BlockchainsApi.md#patch_blockchain_async) | **PATCH** /api/v2/BlockchainsService/Blockchains/{id} | Patch a blockchain
[**patch_blockchain_block_async**](BlockchainsApi.md#patch_blockchain_block_async) | **PATCH** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Patch a blockchain block
[**update_blockchain_async**](BlockchainsApi.md#update_blockchain_async) | **PUT** /api/v2/BlockchainsService/Blockchains/{id} | Update a blockchain
[**update_blockchain_block_async**](BlockchainsApi.md#update_blockchain_block_async) | **PUT** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Update a blockchain block



## create_blockchain_async

> create_blockchain_async(tenant_id, api_version, x_api_version, blockchain_create_dto)
Create a new blockchain

Creates a new blockchain for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_create_dto** | Option<[**BlockchainCreateDto**](BlockchainCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_blockchain_block_async

> create_blockchain_block_async(tenant_id, blockchain_id, api_version, x_api_version, blockchain_block_create_dto)
Add a block to a blockchain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_block_create_dto** | Option<[**BlockchainBlockCreateDto**](BlockchainBlockCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_blockchain_async

> delete_blockchain_async(tenant_id, id, api_version, x_api_version)
Delete a blockchain

Deletes a blockchain for the specified tenant.

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


## delete_blockchain_block_async

> delete_blockchain_block_async(tenant_id, blockchain_id, block_id, api_version, x_api_version)
Delete a blockchain block

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**block_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchain_block_by_id_async

> models::BlockchainBlockDto get_blockchain_block_by_id_async(tenant_id, blockchain_id, block_id, api_version, x_api_version)
Get a specific block

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**block_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlockchainBlockDto**](BlockchainBlockDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchain_blocks_async

> models::BlockchainBlockDtoListEnvelope get_blockchain_blocks_async(tenant_id, blockchain_id, api_version, x_api_version, blockchain_block_dto_collection_query_parameters)
Get blocks for a blockchain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_block_dto_collection_query_parameters** | Option<[**BlockchainBlockDtoCollectionQueryParameters**](BlockchainBlockDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::BlockchainBlockDtoListEnvelope**](BlockchainBlockDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchain_blocks_count_async

> models::Int32Envelope get_blockchain_blocks_count_async(tenant_id, blockchain_id, api_version, x_api_version, blockchain_block_dto_collection_query_parameters)
Get block count for a blockchain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_block_dto_collection_query_parameters** | Option<[**BlockchainBlockDtoCollectionQueryParameters**](BlockchainBlockDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchain_by_id_async

> models::BlockchainDto get_blockchain_by_id_async(tenant_id, id, api_version, x_api_version)
Get blockchain by ID

Retrieves a specific blockchain by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::BlockchainDto**](BlockchainDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchains_async

> models::BlockchainDtoListEnvelope get_blockchains_async(tenant_id, api_version, x_api_version, blockchain_dto_collection_query_parameters)
Get all blockchains

Retrieves all blockchains for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_dto_collection_query_parameters** | Option<[**BlockchainDtoCollectionQueryParameters**](BlockchainDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::BlockchainDtoListEnvelope**](BlockchainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blockchains_count_async

> models::Int32Envelope get_blockchains_count_async(tenant_id, api_version, x_api_version, blockchain_dto_collection_query_parameters)
Get blockchains count

Returns the count of blockchains for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_dto_collection_query_parameters** | Option<[**BlockchainDtoCollectionQueryParameters**](BlockchainDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_blockchain_async

> models::EmptyEnvelope patch_blockchain_async(tenant_id, id, api_version, x_api_version, patch_operation)
Patch a blockchain

Patch a blockchain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_blockchain_block_async

> models::EmptyEnvelope patch_blockchain_block_async(tenant_id, blockchain_id, block_id, api_version, x_api_version, patch_operation)
Patch a blockchain block

Patch a blockchain block

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**block_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_blockchain_async

> update_blockchain_async(tenant_id, id, api_version, x_api_version, blockchain_update_dto)
Update a blockchain

Updates an existing blockchain for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_update_dto** | Option<[**BlockchainUpdateDto**](BlockchainUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_blockchain_block_async

> update_blockchain_block_async(tenant_id, blockchain_id, block_id, api_version, x_api_version, blockchain_block_update_dto)
Update a blockchain block

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**blockchain_id** | **uuid::Uuid** |  | [required] |
**block_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**blockchain_block_update_dto** | Option<[**BlockchainBlockUpdateDto**](BlockchainBlockUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

