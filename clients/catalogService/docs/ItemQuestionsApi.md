# \ItemQuestionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_item_question_async**](ItemQuestionsApi.md#create_item_question_async) | **POST** /api/v2/CatalogService/ItemQuestions | Create a new item question
[**delete_item_question_async**](ItemQuestionsApi.md#delete_item_question_async) | **DELETE** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Delete an item question
[**get_item_question_by_id_async**](ItemQuestionsApi.md#get_item_question_by_id_async) | **GET** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Get item question by ID
[**get_item_questions_async**](ItemQuestionsApi.md#get_item_questions_async) | **GET** /api/v2/CatalogService/ItemQuestions | Get all item questions
[**update_item_question_async**](ItemQuestionsApi.md#update_item_question_async) | **PUT** /api/v2/CatalogService/ItemQuestions/{itemQuestionId} | Update an item question



## create_item_question_async

> models::ItemQuestionDtoEnvelope create_item_question_async(tenant_id, api_version, x_api_version, item_question_create_dto)
Create a new item question

Creates a new item question for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_question_create_dto** | Option<[**ItemQuestionCreateDto**](ItemQuestionCreateDto.md)> |  |  |

### Return type

[**models::ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_item_question_async

> delete_item_question_async(tenant_id, item_question_id, api_version, x_api_version)
Delete an item question

Deletes an item question for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_question_id** | **uuid::Uuid** |  | [required] |
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


## get_item_question_by_id_async

> models::ItemQuestionDtoEnvelope get_item_question_by_id_async(item_question_id, api_version, x_api_version)
Get item question by ID

Retrieves a specific item question by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_question_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_item_questions_async

> models::ItemQuestionDtoListEnvelope get_item_questions_async(tenant_id, api_version, x_api_version)
Get all item questions

Retrieves all item questions for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemQuestionDtoListEnvelope**](ItemQuestionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_item_question_async

> update_item_question_async(tenant_id, item_question_id, api_version, x_api_version, item_question_update_dto)
Update an item question

Updates an existing item question for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_question_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_question_update_dto** | Option<[**ItemQuestionUpdateDto**](ItemQuestionUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

