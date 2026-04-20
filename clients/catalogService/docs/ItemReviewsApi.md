# \ItemReviewsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_review_async**](ItemReviewsApi.md#create_item_review_async) | **POST** /api/v2/CatalogService/ItemReviews | Create a new item review
[**delete_item_review_async**](ItemReviewsApi.md#delete_item_review_async) | **DELETE** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Delete an item review
[**get_item_review_by_id_async**](ItemReviewsApi.md#get_item_review_by_id_async) | **GET** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Get item review by ID
[**get_item_reviews_async**](ItemReviewsApi.md#get_item_reviews_async) | **GET** /api/v2/CatalogService/ItemReviews | Get all item reviews
[**update_item_review_async**](ItemReviewsApi.md#update_item_review_async) | **PUT** /api/v2/CatalogService/ItemReviews/{itemReviewId} | Update an item review



## create_item_review_async

> models::ItemReviewDtoEnvelope create_item_review_async(tenant_id, api_version, x_api_version, item_review_create_dto)
Create a new item review

Creates a new item review for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_review_create_dto** | Option<[**ItemReviewCreateDto**](ItemReviewCreateDto.md)> |  |  |

### Return type

[**models::ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_review_async

> delete_item_review_async(tenant_id, item_review_id, api_version, x_api_version)
Delete an item review

Deletes an item review for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_review_id** | **uuid::Uuid** |  | [required] |
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


## get_item_review_by_id_async

> models::ItemReviewDtoEnvelope get_item_review_by_id_async(item_review_id, api_version, x_api_version)
Get item review by ID

Retrieves a specific item review by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_review_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_reviews_async

> models::ItemReviewDtoListEnvelope get_item_reviews_async(item_id, api_version, x_api_version)
Get all item reviews

Retrieves all item reviews for the specified item using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReviewDtoListEnvelope**](ItemReviewDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_review_async

> update_item_review_async(tenant_id, item_review_id, api_version, x_api_version, item_review_update_dto)
Update an item review

Updates an existing item review for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_review_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_review_update_dto** | Option<[**ItemReviewUpdateDto**](ItemReviewUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

