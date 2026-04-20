# \AssetTransfersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_asset_transfer_async**](AssetTransfersApi.md#create_asset_transfer_async) | **POST** /api/v2/AssetsService/AssetTransfers | Creates a new asset transfer
[**delete_asset_transfer_async**](AssetTransfersApi.md#delete_asset_transfer_async) | **DELETE** /api/v2/AssetsService/AssetTransfers/{transferId} | Deletes an asset transfer
[**get_asset_transfer_async**](AssetTransfersApi.md#get_asset_transfer_async) | **GET** /api/v2/AssetsService/AssetTransfers/{transferId} | Gets a single asset transfer by ID
[**get_asset_transfers_async**](AssetTransfersApi.md#get_asset_transfers_async) | **GET** /api/v2/AssetsService/AssetTransfers | Gets a list of asset transfers
[**get_asset_transfers_count_async**](AssetTransfersApi.md#get_asset_transfers_count_async) | **GET** /api/v2/AssetsService/AssetTransfers/Count | Gets the count of asset transfers
[**update_asset_transfer_async**](AssetTransfersApi.md#update_asset_transfer_async) | **PUT** /api/v2/AssetsService/AssetTransfers/{transferId} | Updates an existing asset transfer



## create_asset_transfer_async

> models::EmptyEnvelope create_asset_transfer_async(tenant_id, asset_transfer_create_dto)
Creates a new asset transfer

Creates a new asset transfer for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_transfer_create_dto** | Option<[**AssetTransferCreateDto**](AssetTransferCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_transfer_async

> models::EmptyEnvelope delete_asset_transfer_async(tenant_id, transfer_id)
Deletes an asset transfer

Deletes an asset transfer for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transfer_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfer_async

> models::AssetTransferDtoEnvelope get_asset_transfer_async(tenant_id, transfer_id)
Gets a single asset transfer by ID

Retrieves a specific asset transfer by its ID for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transfer_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTransferDtoEnvelope**](AssetTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfers_async

> models::AssetTransferDtoListEnvelope get_asset_transfers_async(tenant_id)
Gets a list of asset transfers

Retrieves all asset transfers for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTransferDtoListEnvelope**](AssetTransferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfers_count_async

> models::Int32Envelope get_asset_transfers_count_async(tenant_id)
Gets the count of asset transfers

Returns the total number of asset transfers for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_transfer_async

> models::EmptyEnvelope update_asset_transfer_async(tenant_id, transfer_id, asset_transfer_update_dto)
Updates an existing asset transfer

Updates an existing asset transfer for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**transfer_id** | **uuid::Uuid** |  | [required] |
**asset_transfer_update_dto** | Option<[**AssetTransferUpdateDto**](AssetTransferUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

