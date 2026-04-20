# \AssetsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_asset**](AssetsApi.md#create_asset) | **POST** /api/v2/AssetsService/Assets | Creates a new asset
[**create_asset_asset_category**](AssetsApi.md#create_asset_asset_category) | **POST** /api/v2/AssetsService/Assets/Categories | Creates a new asset category
[**create_asset_depreciation_record**](AssetsApi.md#create_asset_depreciation_record) | **POST** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords | Creates a new depreciation record for an asset
[**create_asset_repair**](AssetsApi.md#create_asset_repair) | **POST** /api/v2/AssetsService/Assets/{assetId}/Repairs | Creates a new repair for an asset
[**create_asset_transfer**](AssetsApi.md#create_asset_transfer) | **POST** /api/v2/AssetsService/Assets/{assetId}/Transfers | Creates a new transfer for an asset
[**create_asset_value_amend**](AssetsApi.md#create_asset_value_amend) | **POST** /api/v2/AssetsService/Assets/{assetId}/ValueAmends | Creates a new value amendment for an asset
[**delete_asset**](AssetsApi.md#delete_asset) | **DELETE** /api/v2/AssetsService/Assets/{assetId} | Deletes an existing asset
[**delete_asset_asset_category**](AssetsApi.md#delete_asset_asset_category) | **DELETE** /api/v2/AssetsService/Assets/Categories/{categoryId} | Deletes an existing asset category
[**delete_asset_depreciation_record**](AssetsApi.md#delete_asset_depreciation_record) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Deletes a depreciation record for an asset
[**delete_asset_repair**](AssetsApi.md#delete_asset_repair) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Deletes a repair for an asset
[**delete_asset_transfer**](AssetsApi.md#delete_asset_transfer) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Deletes a transfer for an asset
[**delete_asset_value_amend**](AssetsApi.md#delete_asset_value_amend) | **DELETE** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Deletes a value amendment for an asset
[**get_asset**](AssetsApi.md#get_asset) | **GET** /api/v2/AssetsService/Assets/{assetId} | Gets a specific asset by ID
[**get_asset_asset_categories**](AssetsApi.md#get_asset_asset_categories) | **GET** /api/v2/AssetsService/Assets/Categories | Gets all asset categories
[**get_asset_asset_categories_count**](AssetsApi.md#get_asset_asset_categories_count) | **GET** /api/v2/AssetsService/Assets/Categories/count | Gets the count of asset categories
[**get_asset_asset_category**](AssetsApi.md#get_asset_asset_category) | **GET** /api/v2/AssetsService/Assets/Categories/{categoryId} | Gets a specific asset category
[**get_asset_depreciation_record**](AssetsApi.md#get_asset_depreciation_record) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Gets a specific depreciation record for an asset
[**get_asset_depreciation_records**](AssetsApi.md#get_asset_depreciation_records) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords | Gets depreciation records for a specific asset
[**get_asset_depreciation_records_count**](AssetsApi.md#get_asset_depreciation_records_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/Count | Gets count of depreciation records for a specific asset
[**get_asset_repair**](AssetsApi.md#get_asset_repair) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Gets a specific repair for an asset
[**get_asset_repairs**](AssetsApi.md#get_asset_repairs) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs | Gets repairs for a specific asset
[**get_asset_repairs_count**](AssetsApi.md#get_asset_repairs_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/Repairs/Count | Gets count of repairs for a specific asset
[**get_asset_transfer**](AssetsApi.md#get_asset_transfer) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Gets a specific transfer for an asset
[**get_asset_transfers**](AssetsApi.md#get_asset_transfers) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers | Gets transfers for a specific asset
[**get_asset_transfers_count**](AssetsApi.md#get_asset_transfers_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/Transfers/Count | Gets count of transfers for a specific asset
[**get_asset_value_amend**](AssetsApi.md#get_asset_value_amend) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Gets a specific value amendment for an asset
[**get_asset_value_amends**](AssetsApi.md#get_asset_value_amends) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends | Gets value amendments for a specific asset
[**get_asset_value_amends_count**](AssetsApi.md#get_asset_value_amends_count) | **GET** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/Count | Gets count of value amendments for a specific asset
[**get_assets**](AssetsApi.md#get_assets) | **GET** /api/v2/AssetsService/Assets | Gets all assets for the current tenant
[**get_assets_count**](AssetsApi.md#get_assets_count) | **GET** /api/v2/AssetsService/Assets/count | Gets the count of assets
[**update_asset**](AssetsApi.md#update_asset) | **PUT** /api/v2/AssetsService/Assets/{assetId} | Updates an existing asset
[**update_asset_asset_category**](AssetsApi.md#update_asset_asset_category) | **PUT** /api/v2/AssetsService/Assets/Categories/{categoryId} | Updates an existing asset category
[**update_asset_depreciation_record**](AssetsApi.md#update_asset_depreciation_record) | **PUT** /api/v2/AssetsService/Assets/{assetId}/DepreciationRecords/{recordId} | Updates a depreciation record for an asset
[**update_asset_repair**](AssetsApi.md#update_asset_repair) | **PUT** /api/v2/AssetsService/Assets/{assetId}/Repairs/{repairId} | Updates a repair for an asset
[**update_asset_transfer**](AssetsApi.md#update_asset_transfer) | **PUT** /api/v2/AssetsService/Assets/{assetId}/Transfers/{transferId} | Updates a transfer for an asset
[**update_asset_value_amend**](AssetsApi.md#update_asset_value_amend) | **PUT** /api/v2/AssetsService/Assets/{assetId}/ValueAmends/{amendId} | Updates a value amendment for an asset



## create_asset

> models::AssetDtoEnvelope create_asset(tenant_id, asset_create_dto)
Creates a new asset

Creates a new asset for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_create_dto** | Option<[**AssetCreateDto**](AssetCreateDto.md)> |  |  |

### Return type

[**models::AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_asset_asset_category

> models::AssetCategoryDtoEnvelope create_asset_asset_category(tenant_id, asset_category_create_dto)
Creates a new asset category

Creates a new asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_category_create_dto** | Option<[**AssetCategoryCreateDto**](AssetCategoryCreateDto.md)> |  |  |

### Return type

[**models::AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_asset_depreciation_record

> models::EmptyEnvelope create_asset_depreciation_record(tenant_id, asset_id, asset_depreciation_record_create_dto)
Creates a new depreciation record for an asset

Creates a new depreciation record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**asset_depreciation_record_create_dto** | Option<[**AssetDepreciationRecordCreateDto**](AssetDepreciationRecordCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_asset_repair

> models::EmptyEnvelope create_asset_repair(tenant_id, asset_id, asset_repair_create_dto)
Creates a new repair for an asset

Creates a new repair record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**asset_repair_create_dto** | Option<[**AssetRepairCreateDto**](AssetRepairCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_asset_transfer

> models::EmptyEnvelope create_asset_transfer(tenant_id, asset_id, asset_transfer_create_dto)
Creates a new transfer for an asset

Creates a new transfer record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**asset_transfer_create_dto** | Option<[**AssetTransferCreateDto**](AssetTransferCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_asset_value_amend

> models::EmptyEnvelope create_asset_value_amend(tenant_id, asset_id, asset_value_amend_create_dto)
Creates a new value amendment for an asset

Creates a new value amendment record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**asset_value_amend_create_dto** | Option<[**AssetValueAmendCreateDto**](AssetValueAmendCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset

> delete_asset(tenant_id, asset_id)
Deletes an existing asset

Deletes an existing asset for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_asset_category

> delete_asset_asset_category(tenant_id, category_id)
Deletes an existing asset category

Deletes an existing asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_depreciation_record

> models::EmptyEnvelope delete_asset_depreciation_record(tenant_id, asset_id, record_id)
Deletes a depreciation record for an asset

Deletes a depreciation record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**record_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_repair

> models::EmptyEnvelope delete_asset_repair(tenant_id, asset_id, repair_id)
Deletes a repair for an asset

Deletes a repair record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**repair_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_transfer

> models::EmptyEnvelope delete_asset_transfer(tenant_id, asset_id, transfer_id)
Deletes a transfer for an asset

Deletes a transfer record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**transfer_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_asset_value_amend

> models::EmptyEnvelope delete_asset_value_amend(tenant_id, asset_id, amend_id)
Deletes a value amendment for an asset

Deletes a value amendment record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**amend_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset

> models::AssetDtoEnvelope get_asset(tenant_id, asset_id)
Gets a specific asset by ID

Retrieves a specific asset for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_asset_categories

> models::AssetCategoryDtoListEnvelope get_asset_asset_categories(tenant_id)
Gets all asset categories

Retrieves all asset categories for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetCategoryDtoListEnvelope**](AssetCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_asset_categories_count

> models::Int32Envelope get_asset_asset_categories_count(tenant_id)
Gets the count of asset categories

Returns the total number of asset categories for the authenticated tenant.

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


## get_asset_asset_category

> models::AssetCategoryDtoEnvelope get_asset_asset_category(tenant_id, category_id)
Gets a specific asset category

Retrieves a specific asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_depreciation_record

> models::AssetDepreciationRecordDtoEnvelope get_asset_depreciation_record(tenant_id, asset_id, record_id)
Gets a specific depreciation record for an asset

Retrieves a specific depreciation record by ID for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**record_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetDepreciationRecordDtoEnvelope**](AssetDepreciationRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_depreciation_records

> models::AssetDepreciationRecordDtoListEnvelope get_asset_depreciation_records(tenant_id, asset_id)
Gets depreciation records for a specific asset

Retrieves all depreciation records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetDepreciationRecordDtoListEnvelope**](AssetDepreciationRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_depreciation_records_count

> models::Int32Envelope get_asset_depreciation_records_count(tenant_id, asset_id)
Gets count of depreciation records for a specific asset

Returns the total number of depreciation records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_repair

> models::AssetRepairDtoEnvelope get_asset_repair(tenant_id, asset_id, repair_id)
Gets a specific repair for an asset

Retrieves a specific repair record by ID for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**repair_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetRepairDtoEnvelope**](AssetRepairDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_repairs

> models::AssetRepairDtoListEnvelope get_asset_repairs(tenant_id, asset_id)
Gets repairs for a specific asset

Retrieves all repair records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetRepairDtoListEnvelope**](AssetRepairDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_repairs_count

> models::Int32Envelope get_asset_repairs_count(tenant_id, asset_id)
Gets count of repairs for a specific asset

Returns the total number of repair records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfer

> models::AssetTransferDtoEnvelope get_asset_transfer(tenant_id, asset_id, transfer_id)
Gets a specific transfer for an asset

Retrieves a specific transfer record by ID for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**transfer_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTransferDtoEnvelope**](AssetTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfers

> models::AssetTransferDtoListEnvelope get_asset_transfers(tenant_id, asset_id)
Gets transfers for a specific asset

Retrieves all transfer records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetTransferDtoListEnvelope**](AssetTransferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_transfers_count

> models::Int32Envelope get_asset_transfers_count(tenant_id, asset_id)
Gets count of transfers for a specific asset

Returns the total number of transfer records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_value_amend

> models::AssetValueAmendDtoEnvelope get_asset_value_amend(tenant_id, asset_id, amend_id)
Gets a specific value amendment for an asset

Retrieves a specific value amendment record by ID for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**amend_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetValueAmendDtoEnvelope**](AssetValueAmendDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_value_amends

> models::AssetValueAmendDtoListEnvelope get_asset_value_amends(tenant_id, asset_id)
Gets value amendments for a specific asset

Retrieves all value amendment records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetValueAmendDtoListEnvelope**](AssetValueAmendDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_asset_value_amends_count

> models::Int32Envelope get_asset_value_amends_count(tenant_id, asset_id)
Gets count of value amendments for a specific asset

Returns the total number of value amendment records for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_assets

> models::AssetDtoListEnvelope get_assets(tenant_id)
Gets all assets for the current tenant

Retrieves all assets for the authenticated tenant with optional filtering.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::AssetDtoListEnvelope**](AssetDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_assets_count

> models::Int32Envelope get_assets_count(tenant_id)
Gets the count of assets

Returns the total number of assets for the authenticated tenant.

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


## update_asset

> models::AssetDtoEnvelope update_asset(tenant_id, asset_id, asset_update_dto)
Updates an existing asset

Updates an existing asset for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**asset_update_dto** | Option<[**AssetUpdateDto**](AssetUpdateDto.md)> |  |  |

### Return type

[**models::AssetDtoEnvelope**](AssetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_asset_category

> models::AssetCategoryDtoEnvelope update_asset_asset_category(tenant_id, category_id, asset_category_update_dto)
Updates an existing asset category

Updates an existing asset category for the authenticated tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**category_id** | **uuid::Uuid** |  | [required] |
**asset_category_update_dto** | Option<[**AssetCategoryUpdateDto**](AssetCategoryUpdateDto.md)> |  |  |

### Return type

[**models::AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_depreciation_record

> models::EmptyEnvelope update_asset_depreciation_record(tenant_id, asset_id, record_id, asset_depreciation_record_update_dto)
Updates a depreciation record for an asset

Updates an existing depreciation record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**record_id** | **uuid::Uuid** |  | [required] |
**asset_depreciation_record_update_dto** | Option<[**AssetDepreciationRecordUpdateDto**](AssetDepreciationRecordUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_repair

> models::EmptyEnvelope update_asset_repair(tenant_id, asset_id, repair_id, asset_repair_update_dto)
Updates a repair for an asset

Updates an existing repair record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**repair_id** | **uuid::Uuid** |  | [required] |
**asset_repair_update_dto** | Option<[**AssetRepairUpdateDto**](AssetRepairUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_asset_transfer

> models::EmptyEnvelope update_asset_transfer(tenant_id, asset_id, transfer_id, asset_transfer_update_dto)
Updates a transfer for an asset

Updates an existing transfer record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
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


## update_asset_value_amend

> models::EmptyEnvelope update_asset_value_amend(tenant_id, asset_id, amend_id, asset_value_amend_update_dto)
Updates a value amendment for an asset

Updates an existing value amendment record for the specified asset.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**asset_id** | **uuid::Uuid** |  | [required] |
**amend_id** | **uuid::Uuid** |  | [required] |
**asset_value_amend_update_dto** | Option<[**AssetValueAmendUpdateDto**](AssetValueAmendUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

