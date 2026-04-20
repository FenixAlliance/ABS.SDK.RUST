# \ItemImagesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_image_async**](ItemImagesApi.md#create_item_image_async) | **POST** /api/v2/CatalogService/ItemImages | Create a new item image
[**delete_item_image_async**](ItemImagesApi.md#delete_item_image_async) | **DELETE** /api/v2/CatalogService/ItemImages/{itemImageId} | Delete an item image
[**get_item_image_by_id_async**](ItemImagesApi.md#get_item_image_by_id_async) | **GET** /api/v2/CatalogService/ItemImages/{itemImageId} | Get item image by ID
[**get_item_images_async**](ItemImagesApi.md#get_item_images_async) | **GET** /api/v2/CatalogService/ItemImages | Get all item images
[**update_item_image_async**](ItemImagesApi.md#update_item_image_async) | **PUT** /api/v2/CatalogService/ItemImages/{itemImageId} | Update an item image



## create_item_image_async

> models::ItemImageDtoEnvelope create_item_image_async(tenant_id, api_version, x_api_version, item_image_create_dto)
Create a new item image

Creates a new item image for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_image_create_dto** | Option<[**ItemImageCreateDto**](ItemImageCreateDto.md)> |  |  |

### Return type

[**models::ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_image_async

> delete_item_image_async(tenant_id, item_image_id, api_version, x_api_version)
Delete an item image

Deletes an item image for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_image_id** | **uuid::Uuid** |  | [required] |
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


## get_item_image_by_id_async

> models::ItemImageDtoEnvelope get_item_image_by_id_async(item_image_id, api_version, x_api_version)
Get item image by ID

Retrieves a specific item image by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_image_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_images_async

> models::ItemImageDtoListEnvelope get_item_images_async(tenant_id, api_version, x_api_version)
Get all item images

Retrieves all item images for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemImageDtoListEnvelope**](ItemImageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_image_async

> update_item_image_async(tenant_id, item_image_id, api_version, x_api_version, item_image_update_dto)
Update an item image

Updates an existing item image for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_image_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_image_update_dto** | Option<[**ItemImageUpdateDto**](ItemImageUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

