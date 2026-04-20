# \DiscountListsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_discount_list**](DiscountListsApi.md#create_discount_list) | **POST** /api/v2/PricingService/DiscountLists | Creates a new discount list
[**create_discount_list_entry**](DiscountListsApi.md#create_discount_list_entry) | **POST** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts | Creates a discount list entry
[**delete_discount_list**](DiscountListsApi.md#delete_discount_list) | **DELETE** /api/v2/PricingService/DiscountLists/{discountListId} | Deletes a discount list
[**delete_discount_list_entry**](DiscountListsApi.md#delete_discount_list_entry) | **DELETE** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Deletes a discount list entry
[**get_discount_list**](DiscountListsApi.md#get_discount_list) | **GET** /api/v2/PricingService/DiscountLists/{discountListId} | Gets a discount list by ID
[**get_discount_list_entries**](DiscountListsApi.md#get_discount_list_entries) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts | Retrieves discounts in a discount list
[**get_discount_list_entries_count**](DiscountListsApi.md#get_discount_list_entries_count) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/Count | Counts discounts in a discount list
[**get_discount_list_entry**](DiscountListsApi.md#get_discount_list_entry) | **GET** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Gets a discount list entry by ID
[**get_discount_lists**](DiscountListsApi.md#get_discount_lists) | **GET** /api/v2/PricingService/DiscountLists | Retrieves all discount lists
[**get_discount_lists_count**](DiscountListsApi.md#get_discount_lists_count) | **GET** /api/v2/PricingService/DiscountLists/Count | Counts discount lists
[**update_discount_list**](DiscountListsApi.md#update_discount_list) | **PUT** /api/v2/PricingService/DiscountLists/{discountListId} | Updates a discount list
[**update_discount_list_entry**](DiscountListsApi.md#update_discount_list_entry) | **PUT** /api/v2/PricingService/DiscountLists/{discountListId}/Discounts/{discountListEntryId} | Updates a discount list entry



## create_discount_list

> models::EmptyEnvelope create_discount_list(tenant_id, discount_list_create_dto)
Creates a new discount list

Creates a new discount list for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_create_dto** | Option<[**DiscountListCreateDto**](DiscountListCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_discount_list_entry

> models::EmptyEnvelope create_discount_list_entry(tenant_id, discount_list_id, discount_create_dto)
Creates a discount list entry

Creates a new discount entry in the specified discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |
**discount_create_dto** | Option<[**DiscountCreateDto**](DiscountCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_discount_list

> models::EmptyEnvelope delete_discount_list(tenant_id, discount_list_id)
Deletes a discount list

Deletes the specified discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_discount_list_entry

> models::EmptyEnvelope delete_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)
Deletes a discount list entry

Deletes the specified discount entry from a discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |
**discount_list_entry_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_list

> models::DiscountListDtoEnvelope get_discount_list(tenant_id, discount_list_id)
Gets a discount list by ID

Retrieves the details of a discount list using its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DiscountListDtoEnvelope**](DiscountListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_list_entries

> models::DiscountDtoListEnvelope get_discount_list_entries(tenant_id, discount_list_id)
Retrieves discounts in a discount list

Gets all discount entries for a specific discount list with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DiscountDtoListEnvelope**](DiscountDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_list_entries_count

> models::Int32Envelope get_discount_list_entries_count(tenant_id, discount_list_id)
Counts discounts in a discount list

Gets the count of discount entries for a specific discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_list_entry

> models::DiscountDtoEnvelope get_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id)
Gets a discount list entry by ID

Retrieves a specific discount entry from a discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |
**discount_list_entry_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DiscountDtoEnvelope**](DiscountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_lists

> models::DiscountListDtoListEnvelope get_discount_lists(tenant_id)
Retrieves all discount lists

Gets all discount lists for the current tenant with OData support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::DiscountListDtoListEnvelope**](DiscountListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_discount_lists_count

> models::Int32Envelope get_discount_lists_count(tenant_id)
Counts discount lists

Gets the count of discount lists for the current tenant.

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


## update_discount_list

> models::EmptyEnvelope update_discount_list(tenant_id, discount_list_id, discount_list_update_dto)
Updates a discount list

Updates the specified discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |
**discount_list_update_dto** | Option<[**DiscountListUpdateDto**](DiscountListUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_discount_list_entry

> models::EmptyEnvelope update_discount_list_entry(tenant_id, discount_list_id, discount_list_entry_id, discount_update_dto)
Updates a discount list entry

Updates the specified discount entry in a discount list.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**discount_list_id** | **uuid::Uuid** |  | [required] |
**discount_list_entry_id** | **uuid::Uuid** |  | [required] |
**discount_update_dto** | Option<[**DiscountUpdateDto**](DiscountUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

