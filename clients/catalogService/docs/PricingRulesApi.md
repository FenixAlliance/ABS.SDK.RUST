# \PricingRulesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_pricing_rule**](PricingRulesApi.md#create_pricing_rule) | **POST** /api/v2/CatalogService/PricingRules | Create a new pricing rule
[**delete_pricing_rule**](PricingRulesApi.md#delete_pricing_rule) | **DELETE** /api/v2/CatalogService/PricingRules/{pricingRuleId} | Delete a pricing rule
[**get_pricing_rule_by_id**](PricingRulesApi.md#get_pricing_rule_by_id) | **GET** /api/v2/CatalogService/PricingRules/{pricingRuleId} | Get pricing rule by ID
[**get_pricing_rules**](PricingRulesApi.md#get_pricing_rules) | **GET** /api/v2/CatalogService/PricingRules | Get all pricing rules
[**update_pricing_rule**](PricingRulesApi.md#update_pricing_rule) | **PUT** /api/v2/CatalogService/PricingRules/Update | Update a pricing rule



## create_pricing_rule

> models::PricingRuleDtoEnvelope create_pricing_rule(tenant_id, api_version, x_api_version, pricing_rule_create_dto)
Create a new pricing rule

Creates a new pricing rule for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**pricing_rule_create_dto** | Option<[**PricingRuleCreateDto**](PricingRuleCreateDto.md)> |  |  |

### Return type

[**models::PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_pricing_rule

> delete_pricing_rule(tenant_id, pricing_rule_id, api_version, x_api_version)
Delete a pricing rule

Deletes a pricing rule for the specified tenant and rule ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pricing_rule_id** | **uuid::Uuid** |  | [required] |
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


## get_pricing_rule_by_id

> models::PricingRuleDtoEnvelope get_pricing_rule_by_id(pricing_rule_id, api_version, x_api_version)
Get pricing rule by ID

Retrieves a pricing rule by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pricing_rule_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PricingRuleDtoEnvelope**](PricingRuleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_pricing_rules

> models::PricingRuleDtoListEnvelope get_pricing_rules(tenant_id, api_version, x_api_version)
Get all pricing rules

Retrieves all pricing rules for the specified tenant, with optional OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::PricingRuleDtoListEnvelope**](PricingRuleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_pricing_rule

> update_pricing_rule(tenant_id, pricing_rule_id, api_version, x_api_version, pricing_rule_update_dto)
Update a pricing rule

Updates an existing pricing rule for the specified tenant and rule ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**pricing_rule_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**pricing_rule_update_dto** | Option<[**PricingRuleUpdateDto**](PricingRuleUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

