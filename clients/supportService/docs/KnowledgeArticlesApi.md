# \KnowledgeArticlesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_knowledge_article_async**](KnowledgeArticlesApi.md#create_knowledge_article_async) | **POST** /api/v2/SupportService/KnowledgeArticles | Create a knowledge article
[**delete_knowledge_article_async**](KnowledgeArticlesApi.md#delete_knowledge_article_async) | **DELETE** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Delete a knowledge article
[**get_knowledge_article_async**](KnowledgeArticlesApi.md#get_knowledge_article_async) | **GET** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Retrieve a knowledge article by ID
[**get_knowledge_articles_async**](KnowledgeArticlesApi.md#get_knowledge_articles_async) | **GET** /api/v2/SupportService/KnowledgeArticles | Retrieve knowledge articles
[**get_knowledge_articles_count_async**](KnowledgeArticlesApi.md#get_knowledge_articles_count_async) | **GET** /api/v2/SupportService/KnowledgeArticles/Count | Get knowledge articles count
[**update_knowledge_article_async**](KnowledgeArticlesApi.md#update_knowledge_article_async) | **PUT** /api/v2/SupportService/KnowledgeArticles/{knowledgeArticleId} | Update a knowledge article



## create_knowledge_article_async

> models::EmptyEnvelope create_knowledge_article_async(tenant_id, api_version, x_api_version, knowledge_article_create_dto)
Create a knowledge article

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**knowledge_article_create_dto** | Option<[**KnowledgeArticleCreateDto**](KnowledgeArticleCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_knowledge_article_async

> models::EmptyEnvelope delete_knowledge_article_async(tenant_id, knowledge_article_id, api_version, x_api_version)
Delete a knowledge article

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**knowledge_article_id** | **uuid::Uuid** |  | [required] |
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


## get_knowledge_article_async

> models::KnowledgeArticleDtoEnvelope get_knowledge_article_async(tenant_id, knowledge_article_id, api_version, x_api_version)
Retrieve a knowledge article by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**knowledge_article_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::KnowledgeArticleDtoEnvelope**](KnowledgeArticleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_knowledge_articles_async

> models::KnowledgeArticleDtoListEnvelope get_knowledge_articles_async(tenant_id, api_version, x_api_version)
Retrieve knowledge articles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::KnowledgeArticleDtoListEnvelope**](KnowledgeArticleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_knowledge_articles_count_async

> models::Int32Envelope get_knowledge_articles_count_async(tenant_id, api_version, x_api_version)
Get knowledge articles count

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


## update_knowledge_article_async

> models::EmptyEnvelope update_knowledge_article_async(tenant_id, knowledge_article_id, api_version, x_api_version, knowledge_article_update_dto)
Update a knowledge article

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**knowledge_article_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**knowledge_article_update_dto** | Option<[**KnowledgeArticleUpdateDto**](KnowledgeArticleUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

