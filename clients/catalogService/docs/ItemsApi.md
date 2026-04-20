# \ItemsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_stock_item_tags_by_item_id**](ItemsApi.md#count_stock_item_tags_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags/Count | Count tags for a stock item
[**count_stock_items_by_business**](ItemsApi.md#count_stock_items_by_business) | **GET** /api/v2/CatalogService/Items/Count | Count stock items by business
[**create_stock_item**](ItemsApi.md#create_stock_item) | **POST** /api/v2/CatalogService/Items | Create a new stock item
[**delete_stock_item**](ItemsApi.md#delete_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId} | Delete a stock item
[**get_extended_stock_item_by_id**](ItemsApi.md#get_extended_stock_item_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Extended | Get extended stock item by ID
[**get_product_primary_image_async**](ItemsApi.md#get_product_primary_image_async) | **GET** /api/v2/CatalogService/Items/{itemId}/Images/Primary | Get item primary image
[**get_stock_item_attachment_by_id**](ItemsApi.md#get_stock_item_attachment_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Get attachment by ID for a stock item
[**get_stock_item_attachments_by_item_id**](ItemsApi.md#get_stock_item_attachments_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Attachments | Get attachments for a stock item
[**get_stock_item_attribute_option_by_id**](ItemsApi.md#get_stock_item_attribute_option_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Get attribute option by ID for a stock item
[**get_stock_item_attribute_options_by_item_id**](ItemsApi.md#get_stock_item_attribute_options_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/AttributeOptions | Get attribute options for a stock item
[**get_stock_item_brand_by_id**](ItemsApi.md#get_stock_item_brand_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Get brand by ID for a stock item
[**get_stock_item_brands_by_item_id**](ItemsApi.md#get_stock_item_brands_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Brands | Get brands for a stock item
[**get_stock_item_by_id**](ItemsApi.md#get_stock_item_by_id) | **GET** /api/v2/CatalogService/Items/{itemId} | Get stock item by ID
[**get_stock_item_categories_by_item_id**](ItemsApi.md#get_stock_item_categories_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Categories | Get categories for a stock item
[**get_stock_item_category_by_id**](ItemsApi.md#get_stock_item_category_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Get category by ID for a stock item
[**get_stock_item_google_categories_by_item_id**](ItemsApi.md#get_stock_item_google_categories_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/GoogleCategories | Get Google categories for a stock item
[**get_stock_item_google_category_by_id**](ItemsApi.md#get_stock_item_google_category_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Get Google category by ID for a stock item
[**get_stock_item_image_by_id**](ItemsApi.md#get_stock_item_image_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Get image by ID for a stock item
[**get_stock_item_images_by_item_id**](ItemsApi.md#get_stock_item_images_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Images | Get images for a stock item
[**get_stock_item_price_rule_by_id**](ItemsApi.md#get_stock_item_price_rule_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Get price rule by ID for a stock item
[**get_stock_item_price_rules_by_item_id**](ItemsApi.md#get_stock_item_price_rules_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/PriceRules | Get price rules for a stock item
[**get_stock_item_question_by_id**](ItemsApi.md#get_stock_item_question_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Questions/{itemQuestionId} | Get question by ID for a stock item
[**get_stock_item_questions_by_item_id**](ItemsApi.md#get_stock_item_questions_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Questions | Get questions for a stock item
[**get_stock_item_refund_policies_by_item_id**](ItemsApi.md#get_stock_item_refund_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/RefundPolicies | Get refund policies for a stock item
[**get_stock_item_refund_policy_by_id**](ItemsApi.md#get_stock_item_refund_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Get refund policy by ID for a stock item
[**get_stock_item_return_policies_by_item_id**](ItemsApi.md#get_stock_item_return_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies | Get return policies for a stock item
[**get_stock_item_return_policy_by_id**](ItemsApi.md#get_stock_item_return_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Get return policy by ID for a stock item
[**get_stock_item_review_by_id**](ItemsApi.md#get_stock_item_review_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Reviews/{itemReviewId} | Get review by ID for a stock item
[**get_stock_item_reviews_by_item_id**](ItemsApi.md#get_stock_item_reviews_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Reviews | Get reviews for a stock item
[**get_stock_item_shipping_policies_by_item_id**](ItemsApi.md#get_stock_item_shipping_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies | Get shipping policies for a stock item
[**get_stock_item_shipping_policy_by_id**](ItemsApi.md#get_stock_item_shipping_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Get shipping policy by ID for a stock item
[**get_stock_item_tag_by_id**](ItemsApi.md#get_stock_item_tag_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Get tag by ID for a stock item
[**get_stock_item_tags_by_item_id**](ItemsApi.md#get_stock_item_tags_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Tags | Get tags for a stock item
[**get_stock_item_tax_policies_by_item_id**](ItemsApi.md#get_stock_item_tax_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/TaxPolicies | Get tax policies for a stock item
[**get_stock_item_tax_policy_by_id**](ItemsApi.md#get_stock_item_tax_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Get tax policy by ID for a stock item
[**get_stock_item_type_by_id**](ItemsApi.md#get_stock_item_type_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Get type by ID for a stock item
[**get_stock_item_types_by_item_id**](ItemsApi.md#get_stock_item_types_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/Types | Get types for a stock item
[**get_stock_item_warranty_policies_by_item_id**](ItemsApi.md#get_stock_item_warranty_policies_by_item_id) | **GET** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies | Get warranty policies for a stock item
[**get_stock_item_warranty_policy_by_id**](ItemsApi.md#get_stock_item_warranty_policy_by_id) | **GET** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Get warranty policy by ID for a stock item
[**get_stock_items_odata_max_price**](ItemsApi.md#get_stock_items_odata_max_price) | **GET** /api/v2/CatalogService/Items/MaxPrice | Get max price of stock items
[**get_stock_items_odata_min_price**](ItemsApi.md#get_stock_items_odata_min_price) | **GET** /api/v2/CatalogService/Items/MinPrice | Get min price of stock items
[**get_stock_items_query**](ItemsApi.md#get_stock_items_query) | **GET** /api/v2/CatalogService/Items | Get all stock items
[**relate_attachment_to_stock_item**](ItemsApi.md#relate_attachment_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Relate attachment to stock item
[**relate_attribute_option_to_stock_item**](ItemsApi.md#relate_attribute_option_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Relate attribute option to stock item
[**relate_brand_to_stock_item**](ItemsApi.md#relate_brand_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Relate brand to stock item
[**relate_category_to_stock_item**](ItemsApi.md#relate_category_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Relate category to stock item
[**relate_google_category_to_stock_item**](ItemsApi.md#relate_google_category_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Relate Google category to stock item
[**relate_image_to_stock_item**](ItemsApi.md#relate_image_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Relate image to stock item
[**relate_price_rule_to_stock_item**](ItemsApi.md#relate_price_rule_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Relate price rule to stock item
[**relate_question_to_stock_item**](ItemsApi.md#relate_question_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Questions | Create question for stock item
[**relate_refund_policy_to_stock_item**](ItemsApi.md#relate_refund_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Relate refund policy to stock item
[**relate_return_policy_to_stock_item**](ItemsApi.md#relate_return_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Relate return policy to stock item
[**relate_review_to_stock_item**](ItemsApi.md#relate_review_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Reviews | Create review for stock item
[**relate_shipping_policy_to_stock_item**](ItemsApi.md#relate_shipping_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Relate shipping policy to stock item
[**relate_tag_to_stock_item**](ItemsApi.md#relate_tag_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Relate tag to stock item
[**relate_tax_policy_to_stock_item**](ItemsApi.md#relate_tax_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Relate tax policy to stock item
[**relate_type_to_stock_item**](ItemsApi.md#relate_type_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Relate type to stock item
[**relate_warranty_policy_to_stock_item**](ItemsApi.md#relate_warranty_policy_to_stock_item) | **POST** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Relate warranty policy to stock item
[**remove_attachment_from_stock_item**](ItemsApi.md#remove_attachment_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Attachments/{itemAttachmentId} | Remove attachment from stock item
[**remove_attribute_option_from_stock_item**](ItemsApi.md#remove_attribute_option_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/AttributeOptions/{itemAttributeOptionId} | Remove attribute option from stock item
[**remove_brand_from_stock_item**](ItemsApi.md#remove_brand_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Brands/{itemBrandId} | Remove brand from stock item
[**remove_category_from_stock_item**](ItemsApi.md#remove_category_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Categories/{itemCategoryId} | Remove category from stock item
[**remove_google_category_from_stock_item**](ItemsApi.md#remove_google_category_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/GoogleCategories/{itemGoogleCategoryId} | Remove Google category from stock item
[**remove_image_from_stock_item**](ItemsApi.md#remove_image_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Images/{itemImageId} | Remove image from stock item
[**remove_price_rule_from_stock_item**](ItemsApi.md#remove_price_rule_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/PriceRules/{itemPriceRuleId} | Remove price rule from stock item
[**remove_question_from_stock_item**](ItemsApi.md#remove_question_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Questions/{itemQuestionId} | Remove question from stock item
[**remove_refund_policy_from_stock_item**](ItemsApi.md#remove_refund_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/RefundPolicies/{itemRefundPolicyId} | Remove refund policy from stock item
[**remove_return_policy_from_stock_item**](ItemsApi.md#remove_return_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/ReturnPolicies/{itemReturnPolicyId} | Remove return policy from stock item
[**remove_review_from_stock_item**](ItemsApi.md#remove_review_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Reviews/{itemReviewId} | Remove review from stock item
[**remove_shipping_policy_from_stock_item**](ItemsApi.md#remove_shipping_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/ShippingPolicies/{itemShippingPolicyId} | Remove shipping policy from stock item
[**remove_tag_from_stock_item**](ItemsApi.md#remove_tag_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Tags/{itemTagId} | Remove tag from stock item
[**remove_tax_policy_from_stock_item**](ItemsApi.md#remove_tax_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/TaxPolicies/{itemTaxPolicyId} | Remove tax policy from stock item
[**remove_type_from_stock_item**](ItemsApi.md#remove_type_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/Types/{itemTypeId} | Remove type from stock item
[**remove_warranty_policy_from_stock_item**](ItemsApi.md#remove_warranty_policy_from_stock_item) | **DELETE** /api/v2/CatalogService/Items/{itemId}/WarrantyPolicies/{itemWarrantyPolicyId} | Remove warranty policy from stock item
[**update_product_primary_image_async**](ItemsApi.md#update_product_primary_image_async) | **POST** /api/v2/CatalogService/Items/{itemId}/Images/Primary | Update item primary image
[**update_stock_item**](ItemsApi.md#update_stock_item) | **PUT** /api/v2/CatalogService/Items/{itemId} | Update a stock item



## count_stock_item_tags_by_item_id

> models::Int32Envelope count_stock_item_tags_by_item_id(item_id, api_version, x_api_version)
Count tags for a stock item

Counts the number of tags associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## count_stock_items_by_business

> models::Int32Envelope count_stock_items_by_business(tenant_id, api_version, x_api_version)
Count stock items by business

Counts the number of stock items for a business, optionally filtered by tenant and OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
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


## create_stock_item

> create_stock_item(tenant_id, api_version, x_api_version, catalog_item_create_dto)
Create a new stock item

Creates a new stock item for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**catalog_item_create_dto** | Option<[**CatalogItemCreateDto**](CatalogItemCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_stock_item

> delete_stock_item(tenant_id, item_id, api_version, x_api_version)
Delete a stock item

Deletes a stock item for the specified tenant and item ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_extended_stock_item_by_id

> models::CatalogItemDtoEnvelope get_extended_stock_item_by_id(item_id, api_version, x_api_version)
Get extended stock item by ID

Retrieves extended information for a stock item by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CatalogItemDtoEnvelope**](CatalogItemDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_product_primary_image_async

> models::EmptyEnvelope get_product_primary_image_async(item_id, api_version, x_api_version)
Get item primary image

Retrieves the primary image for a specific catalog item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_attachment_by_id

> models::ItemAttachmentDtoEnvelope get_stock_item_attachment_by_id(item_id, item_attachment_id, api_version, x_api_version)
Get attachment by ID for a stock item

Retrieves a specific attachment by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_attachments_by_item_id

> models::ItemAttachmentDtoListEnvelope get_stock_item_attachments_by_item_id(item_id, api_version, x_api_version)
Get attachments for a stock item

Retrieves all attachments associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttachmentDtoListEnvelope**](ItemAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_attribute_option_by_id

> models::ItemAttributeOptionDtoEnvelope get_stock_item_attribute_option_by_id(item_id, item_attribute_option_id, api_version, x_api_version)
Get attribute option by ID for a stock item

Retrieves a specific attribute option by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_attribute_options_by_item_id

> models::ItemAttributeOptionDtoListEnvelope get_stock_item_attribute_options_by_item_id(item_id, api_version, x_api_version)
Get attribute options for a stock item

Retrieves all attribute options associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoListEnvelope**](ItemAttributeOptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_brand_by_id

> models::ItemBrandDtoEnvelope get_stock_item_brand_by_id(item_id, item_brand_id, api_version, x_api_version)
Get brand by ID for a stock item

Retrieves a specific brand by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_brand_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_brands_by_item_id

> models::ItemBrandDtoListEnvelope get_stock_item_brands_by_item_id(item_id, api_version, x_api_version)
Get brands for a stock item

Retrieves all brands associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoListEnvelope**](ItemBrandDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_by_id

> models::CatalogItemDtoEnvelope get_stock_item_by_id(item_id, api_version, x_api_version)
Get stock item by ID

Retrieves a stock item by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CatalogItemDtoEnvelope**](CatalogItemDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_categories_by_item_id

> models::ItemCategoryDtoListEnvelope get_stock_item_categories_by_item_id(item_id, api_version, x_api_version)
Get categories for a stock item

Retrieves all categories associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoListEnvelope**](ItemCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_category_by_id

> models::ItemCategoryDtoEnvelope get_stock_item_category_by_id(item_id, item_category_id, api_version, x_api_version)
Get category by ID for a stock item

Retrieves a specific category by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_google_categories_by_item_id

> models::ItemGoogleCategoryDtoListEnvelope get_stock_item_google_categories_by_item_id(item_id, api_version, x_api_version)
Get Google categories for a stock item

Retrieves all Google categories associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_google_category_by_id

> models::ItemGoogleCategoryDtoEnvelope get_stock_item_google_category_by_id(item_id, item_google_category_id, api_version, x_api_version)
Get Google category by ID for a stock item

Retrieves a specific Google category by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_google_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_image_by_id

> models::ItemImageDtoEnvelope get_stock_item_image_by_id(item_id, item_image_id, api_version, x_api_version)
Get image by ID for a stock item

Retrieves a specific image by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_images_by_item_id

> models::ItemImageDtoListEnvelope get_stock_item_images_by_item_id(item_id, api_version, x_api_version)
Get images for a stock item

Retrieves all images associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_price_rule_by_id

> models::PricingRuleDtoEnvelope get_stock_item_price_rule_by_id(item_id, item_price_rule_id, api_version, x_api_version)
Get price rule by ID for a stock item

Retrieves a specific pricing rule by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_price_rule_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_price_rules_by_item_id

> models::PricingRuleDtoListEnvelope get_stock_item_price_rules_by_item_id(item_id, api_version, x_api_version)
Get price rules for a stock item

Retrieves all pricing rules associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_question_by_id

> models::ItemQuestionDtoEnvelope get_stock_item_question_by_id(item_id, item_question_id, api_version, x_api_version)
Get question by ID for a stock item

Retrieves a specific question by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_questions_by_item_id

> models::ItemQuestionDtoListEnvelope get_stock_item_questions_by_item_id(item_id, api_version, x_api_version)
Get questions for a stock item

Retrieves all questions associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_refund_policies_by_item_id

> models::ItemRefundPolicyDtoListEnvelope get_stock_item_refund_policies_by_item_id(item_id, api_version, x_api_version)
Get refund policies for a stock item

Retrieves all refund policies associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoListEnvelope**](ItemRefundPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_refund_policy_by_id

> models::ItemRefundPolicyDtoEnvelope get_stock_item_refund_policy_by_id(item_id, item_refund_policy_id, api_version, x_api_version)
Get refund policy by ID for a stock item

Retrieves a specific refund policy by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_refund_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_return_policies_by_item_id

> models::ItemReturnPolicyDtoListEnvelope get_stock_item_return_policies_by_item_id(item_id, api_version, x_api_version)
Get return policies for a stock item

Retrieves all return policies associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoListEnvelope**](ItemReturnPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_return_policy_by_id

> models::ItemReturnPolicyDtoEnvelope get_stock_item_return_policy_by_id(item_id, item_return_policy_id, api_version, x_api_version)
Get return policy by ID for a stock item

Retrieves a specific return policy by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_review_by_id

> models::ItemReviewDtoEnvelope get_stock_item_review_by_id(item_id, item_review_id, api_version, x_api_version)
Get review by ID for a stock item

Retrieves a specific review by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
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


## get_stock_item_reviews_by_item_id

> models::ItemReviewDtoListEnvelope get_stock_item_reviews_by_item_id(item_id, api_version, x_api_version)
Get reviews for a stock item

Retrieves all reviews associated with a specific stock item.

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


## get_stock_item_shipping_policies_by_item_id

> models::ItemShippingPolicyDtoListEnvelope get_stock_item_shipping_policies_by_item_id(item_id, api_version, x_api_version)
Get shipping policies for a stock item

Retrieves all shipping policies associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoListEnvelope**](ItemShippingPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_shipping_policy_by_id

> models::ItemShippingPolicyDtoEnvelope get_stock_item_shipping_policy_by_id(item_id, item_shipping_policy_id, api_version, x_api_version)
Get shipping policy by ID for a stock item

Retrieves a specific shipping policy by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_shipping_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_tag_by_id

> models::ItemTagDtoEnvelope get_stock_item_tag_by_id(item_id, item_tag_id, api_version, x_api_version)
Get tag by ID for a stock item

Retrieves a specific tag by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_tags_by_item_id

> models::ItemTagDtoListEnvelope get_stock_item_tags_by_item_id(item_id, api_version, x_api_version)
Get tags for a stock item

Retrieves all tags associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoListEnvelope**](ItemTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_tax_policies_by_item_id

> models::ItemTaxPolicyDtoListEnvelope get_stock_item_tax_policies_by_item_id(item_id, api_version, x_api_version)
Get tax policies for a stock item

Retrieves all tax policies associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyDtoListEnvelope**](ItemTaxPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_tax_policy_by_id

> models::ItemTaxPolicyDtoEnvelope get_stock_item_tax_policy_by_id(item_id, item_tax_policy_id, api_version, x_api_version)
Get tax policy by ID for a stock item

Retrieves a specific tax policy by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_type_by_id

> models::ItemTypeDtoEnvelope get_stock_item_type_by_id(item_id, item_type_id, api_version, x_api_version)
Get type by ID for a stock item

Retrieves a specific type by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_types_by_item_id

> models::ItemTypeDtoListEnvelope get_stock_item_types_by_item_id(item_id, api_version, x_api_version)
Get types for a stock item

Retrieves all types associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoListEnvelope**](ItemTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_warranty_policies_by_item_id

> models::ItemWarrantyPolicyDtoListEnvelope get_stock_item_warranty_policies_by_item_id(item_id, api_version, x_api_version)
Get warranty policies for a stock item

Retrieves all warranty policies associated with a specific stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoListEnvelope**](ItemWarrantyPolicyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_item_warranty_policy_by_id

> models::ItemWarrantyPolicyDtoEnvelope get_stock_item_warranty_policy_by_id(item_id, item_warranty_policy_id, api_version, x_api_version)
Get warranty policy by ID for a stock item

Retrieves a specific warranty policy by ID for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_warranty_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_items_odata_max_price

> models::MoneyEnvelope get_stock_items_odata_max_price(tenant_id, api_version, x_api_version)
Get max price of stock items

Retrieves the maximum price among all stock items, optionally filtered by tenant and OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_items_odata_min_price

> models::MoneyEnvelope get_stock_items_odata_min_price(tenant_id, api_version, x_api_version)
Get min price of stock items

Retrieves the minimum price among all stock items, optionally filtered by tenant and OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_stock_items_query

> models::CatalogItemDtoListEnvelope get_stock_items_query(tenant_id, api_version, x_api_version)
Get all stock items

Retrieves all stock items, optionally filtered by tenant and OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CatalogItemDtoListEnvelope**](CatalogItemDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_attachment_to_stock_item

> models::ItemAttachmentDtoEnvelope relate_attachment_to_stock_item(tenant_id, item_id, item_attachment_id, api_version, x_api_version, item_attachment_create_dto)
Relate attachment to stock item

Associates an attachment with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_attachment_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_attachment_create_dto** | Option<[**ItemAttachmentCreateDto**](ItemAttachmentCreateDto.md)> |  |  |

### Return type

[**models::ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_attribute_option_to_stock_item

> models::ItemAttributeOptionDtoEnvelope relate_attribute_option_to_stock_item(item_id, item_attribute_option_id, api_version, x_api_version)
Relate attribute option to stock item

Associates an attribute option with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_brand_to_stock_item

> models::ItemBrandDtoEnvelope relate_brand_to_stock_item(tenant_id, item_id, item_brand_id, api_version, x_api_version)
Relate brand to stock item

Associates a brand with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_brand_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_category_to_stock_item

> models::ItemCategoryDtoEnvelope relate_category_to_stock_item(tenant_id, item_id, item_category_id, api_version, x_api_version)
Relate category to stock item

Associates a category with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_google_category_to_stock_item

> models::ItemGoogleCategoryDtoEnvelope relate_google_category_to_stock_item(tenant_id, item_id, item_google_category_id, api_version, x_api_version)
Relate Google category to stock item

Associates a Google category with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_google_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_image_to_stock_item

> models::ItemImageDtoEnvelope relate_image_to_stock_item(tenant_id, item_id, item_image_id, api_version, x_api_version)
Relate image to stock item

Associates an image with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
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


## relate_price_rule_to_stock_item

> models::PricingRuleDtoEnvelope relate_price_rule_to_stock_item(item_id, item_price_rule_id, api_version, x_api_version)
Relate price rule to stock item

Associates a pricing rule with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_price_rule_id** | **uuid::Uuid** |  | [required] |
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


## relate_question_to_stock_item

> models::ItemQuestionDtoEnvelope relate_question_to_stock_item(tenant_id, item_id, api_version, x_api_version, item_question_record_create_dto)
Create question for stock item

Creates a new question for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_question_record_create_dto** | Option<[**ItemQuestionRecordCreateDto**](ItemQuestionRecordCreateDto.md)> |  |  |

### Return type

[**models::ItemQuestionDtoEnvelope**](ItemQuestionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_refund_policy_to_stock_item

> models::ItemRefundPolicyDtoEnvelope relate_refund_policy_to_stock_item(tenant_id, item_id, item_refund_policy_id, api_version, x_api_version)
Relate refund policy to stock item

Associates a refund policy with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_refund_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_return_policy_to_stock_item

> models::ItemReturnPolicyDtoEnvelope relate_return_policy_to_stock_item(tenant_id, item_id, item_return_policy_id, api_version, x_api_version)
Relate return policy to stock item

Associates a return policy with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_review_to_stock_item

> models::ItemReviewDtoEnvelope relate_review_to_stock_item(tenant_id, item_id, api_version, x_api_version, item_review_record_create_dto)
Create review for stock item

Creates a new review for a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**item_review_record_create_dto** | Option<[**ItemReviewRecordCreateDto**](ItemReviewRecordCreateDto.md)> |  |  |

### Return type

[**models::ItemReviewDtoEnvelope**](ItemReviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_shipping_policy_to_stock_item

> models::ItemShippingPolicyDtoEnvelope relate_shipping_policy_to_stock_item(tenant_id, item_id, item_shipping_policy_id, api_version, x_api_version)
Relate shipping policy to stock item

Associates a shipping policy with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_shipping_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_tag_to_stock_item

> models::ItemTagDtoEnvelope relate_tag_to_stock_item(tenant_id, item_id, item_tag_id, api_version, x_api_version)
Relate tag to stock item

Associates a tag with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_tax_policy_to_stock_item

> models::ItemTaxPolicyDtoEnvelope relate_tax_policy_to_stock_item(tenant_id, item_id, item_tax_policy_id, api_version, x_api_version)
Relate tax policy to stock item

Associates a tax policy with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_type_to_stock_item

> models::ItemTypeDtoEnvelope relate_type_to_stock_item(tenant_id, item_id, item_type_id, api_version, x_api_version)
Relate type to stock item

Associates a type with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## relate_warranty_policy_to_stock_item

> models::ItemWarrantyPolicyDtoEnvelope relate_warranty_policy_to_stock_item(tenant_id, item_id, item_warranty_policy_id, api_version, x_api_version)
Relate warranty policy to stock item

Associates a warranty policy with a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_warranty_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_attachment_from_stock_item

> models::ItemAttachmentDtoEnvelope remove_attachment_from_stock_item(tenant_id, item_id, item_attachment_id, api_version, x_api_version)
Remove attachment from stock item

Removes an attachment from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_attachment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_attribute_option_from_stock_item

> models::ItemAttributeOptionDtoEnvelope remove_attribute_option_from_stock_item(item_id, item_attribute_option_id, api_version, x_api_version)
Remove attribute option from stock item

Removes an attribute option from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_attribute_option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_brand_from_stock_item

> models::ItemBrandDtoEnvelope remove_brand_from_stock_item(tenant_id, item_id, item_brand_id, api_version, x_api_version)
Remove brand from stock item

Removes a brand association from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_brand_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_category_from_stock_item

> models::ItemCategoryDtoEnvelope remove_category_from_stock_item(tenant_id, item_id, item_category_id, api_version, x_api_version)
Remove category from stock item

Removes a category association from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_google_category_from_stock_item

> models::ItemGoogleCategoryDtoEnvelope remove_google_category_from_stock_item(tenant_id, item_id, item_google_category_id, api_version, x_api_version)
Remove Google category from stock item

Removes a Google category from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_google_category_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_image_from_stock_item

> models::ItemImageDtoEnvelope remove_image_from_stock_item(tenant_id, item_id, item_image_id, api_version, x_api_version)
Remove image from stock item

Removes an image association from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
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


## remove_price_rule_from_stock_item

> models::PricingRuleDtoEnvelope remove_price_rule_from_stock_item(item_id, item_price_rule_id, api_version, x_api_version)
Remove price rule from stock item

Removes a pricing rule from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**item_price_rule_id** | **uuid::Uuid** |  | [required] |
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


## remove_question_from_stock_item

> models::ItemQuestionDtoEnvelope remove_question_from_stock_item(tenant_id, item_id, item_question_id, api_version, x_api_version)
Remove question from stock item

Removes a question from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
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


## remove_refund_policy_from_stock_item

> models::ItemRefundPolicyDtoEnvelope remove_refund_policy_from_stock_item(tenant_id, item_id, item_refund_policy_id, api_version, x_api_version)
Remove refund policy from stock item

Removes a refund policy from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_refund_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemRefundPolicyDtoEnvelope**](ItemRefundPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_return_policy_from_stock_item

> models::ItemReturnPolicyDtoEnvelope remove_return_policy_from_stock_item(tenant_id, item_id, item_return_policy_id, api_version, x_api_version)
Remove return policy from stock item

Removes a return policy from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_return_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemReturnPolicyDtoEnvelope**](ItemReturnPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_review_from_stock_item

> models::ItemReviewDtoEnvelope remove_review_from_stock_item(tenant_id, item_id, item_review_id, api_version, x_api_version)
Remove review from stock item

Removes a review from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
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


## remove_shipping_policy_from_stock_item

> models::ItemShippingPolicyDtoEnvelope remove_shipping_policy_from_stock_item(tenant_id, item_id, item_shipping_policy_id, api_version, x_api_version)
Remove shipping policy from stock item

Removes a shipping policy from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_shipping_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemShippingPolicyDtoEnvelope**](ItemShippingPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_tag_from_stock_item

> models::ItemTagDtoEnvelope remove_tag_from_stock_item(tenant_id, item_id, item_tag_id, api_version, x_api_version)
Remove tag from stock item

Removes a tag association from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_tag_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_tax_policy_from_stock_item

> models::ItemTaxPolicyDtoEnvelope remove_tax_policy_from_stock_item(tenant_id, item_id, item_tax_policy_id, api_version, x_api_version)
Remove tax policy from stock item

Removes a tax policy from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_tax_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTaxPolicyDtoEnvelope**](ItemTaxPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_type_from_stock_item

> models::ItemTypeDtoEnvelope remove_type_from_stock_item(tenant_id, item_id, item_type_id, api_version, x_api_version)
Remove type from stock item

Removes a type association from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_warranty_policy_from_stock_item

> models::ItemWarrantyPolicyDtoEnvelope remove_warranty_policy_from_stock_item(tenant_id, item_id, item_warranty_policy_id, api_version, x_api_version)
Remove warranty policy from stock item

Removes a warranty policy from a stock item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**item_warranty_policy_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ItemWarrantyPolicyDtoEnvelope**](ItemWarrantyPolicyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_product_primary_image_async

> models::EmptyEnvelope update_product_primary_image_async(item_id, tenant_id, api_version, x_api_version, data)
Update item primary image

Updates the primary image for a specific catalog item.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**item_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**data** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_stock_item

> update_stock_item(tenant_id, item_id, api_version, x_api_version, catalog_item_update_dto)
Update a stock item

Updates an existing stock item for the specified tenant and item ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**item_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**catalog_item_update_dto** | Option<[**CatalogItemUpdateDto**](CatalogItemUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

