# \CostCentresApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_cost_centre**](CostCentresApi.md#create_cost_centre) | **POST** /api/v2/AccountingService/CostCentres | Create a cost centre
[**create_cost_centre_budget**](CostCentresApi.md#create_cost_centre_budget) | **POST** /api/v2/AccountingService/CostCentres/CostCentreBudgets | Create a cost centre budget
[**create_cost_centre_group**](CostCentresApi.md#create_cost_centre_group) | **POST** /api/v2/AccountingService/CostCentres/CostCentreGroups | Create a cost centre group
[**delete_cost_centre**](CostCentresApi.md#delete_cost_centre) | **DELETE** /api/v2/AccountingService/CostCentres/{costCentreId} | Delete a cost centre
[**delete_cost_centre_budget**](CostCentresApi.md#delete_cost_centre_budget) | **DELETE** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Delete a cost centre budget
[**delete_cost_centre_group**](CostCentresApi.md#delete_cost_centre_group) | **DELETE** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Delete a cost centre group
[**get_cost_centre**](CostCentresApi.md#get_cost_centre) | **GET** /api/v2/AccountingService/CostCentres/{costCentreId} | Get a cost centre by id
[**get_cost_centre_budget**](CostCentresApi.md#get_cost_centre_budget) | **GET** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Get a cost centre budget by id
[**get_cost_centre_budgets**](CostCentresApi.md#get_cost_centre_budgets) | **GET** /api/v2/AccountingService/CostCentres/CostCentreBudgets | Get all cost centre budgets for a tenant
[**get_cost_centre_group**](CostCentresApi.md#get_cost_centre_group) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Get a cost centre group by id
[**get_cost_centre_groups**](CostCentresApi.md#get_cost_centre_groups) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups | Get all cost centre groups for a tenant
[**get_cost_centre_groups_count**](CostCentresApi.md#get_cost_centre_groups_count) | **GET** /api/v2/AccountingService/CostCentres/CostCentreGroups/Count | Get the count of cost centre groups for a tenant
[**get_cost_centres**](CostCentresApi.md#get_cost_centres) | **GET** /api/v2/AccountingService/CostCentres | Get all cost centres for a tenant
[**get_cost_centres_count**](CostCentresApi.md#get_cost_centres_count) | **GET** /api/v2/AccountingService/CostCentres/Count | Get the count of cost centres for a tenant
[**update_cost_centre**](CostCentresApi.md#update_cost_centre) | **PUT** /api/v2/AccountingService/CostCentres/{costCentreId} | Update a cost centre
[**update_cost_centre_budget**](CostCentresApi.md#update_cost_centre_budget) | **PUT** /api/v2/AccountingService/CostCentres/CostCentreBudgets/{budgetId} | Update a cost centre budget
[**update_cost_centre_group**](CostCentresApi.md#update_cost_centre_group) | **PUT** /api/v2/AccountingService/CostCentres/CostCentreGroups/{groupId} | Update a cost centre group



## create_cost_centre

> models::EmptyEnvelope create_cost_centre(tenant_id, cost_centre_create_dto, api_version, x_api_version)
Create a cost centre

Creates a new cost centre.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_create_dto** | [**CostCentreCreateDto**](CostCentreCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_cost_centre_budget

> models::EmptyEnvelope create_cost_centre_budget(tenant_id, cost_centre_budget_create_dto, api_version, x_api_version)
Create a cost centre budget

Creates a new cost centre budget.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_budget_create_dto** | [**CostCentreBudgetCreateDto**](CostCentreBudgetCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_cost_centre_group

> models::EmptyEnvelope create_cost_centre_group(tenant_id, cost_centre_group_create_dto, api_version, x_api_version)
Create a cost centre group

Creates a new cost centre group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_group_create_dto** | [**CostCentreGroupCreateDto**](CostCentreGroupCreateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_cost_centre

> models::EmptyEnvelope delete_cost_centre(tenant_id, cost_centre_id, api_version, x_api_version)
Delete a cost centre

Deletes a cost centre.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_id** | **uuid::Uuid** |  | [required] |
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


## delete_cost_centre_budget

> models::EmptyEnvelope delete_cost_centre_budget(tenant_id, budget_id, api_version, x_api_version)
Delete a cost centre budget

Deletes a cost centre budget.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**budget_id** | **uuid::Uuid** |  | [required] |
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


## delete_cost_centre_group

> models::EmptyEnvelope delete_cost_centre_group(tenant_id, group_id, api_version, x_api_version)
Delete a cost centre group

Deletes a cost centre group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**group_id** | **uuid::Uuid** |  | [required] |
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


## get_cost_centre

> models::CostCentreDtoEnvelope get_cost_centre(tenant_id, cost_centre_id, api_version, x_api_version)
Get a cost centre by id

Retrieves a cost centre by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreDtoEnvelope**](CostCentreDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centre_budget

> models::CostCentreBudgetDtoEnvelope get_cost_centre_budget(tenant_id, budget_id, api_version, x_api_version)
Get a cost centre budget by id

Retrieves a cost centre budget by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**budget_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreBudgetDtoEnvelope**](CostCentreBudgetDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centre_budgets

> models::CostCentreBudgetDtoListEnvelope get_cost_centre_budgets(tenant_id, api_version, x_api_version)
Get all cost centre budgets for a tenant

Retrieves all cost centre budgets for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreBudgetDtoListEnvelope**](CostCentreBudgetDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centre_group

> models::CostCentreGroupDtoEnvelope get_cost_centre_group(tenant_id, group_id, api_version, x_api_version)
Get a cost centre group by id

Retrieves a cost centre group by its identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**group_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreGroupDtoEnvelope**](CostCentreGroupDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centre_groups

> models::CostCentreGroupDtoListEnvelope get_cost_centre_groups(tenant_id, api_version, x_api_version)
Get all cost centre groups for a tenant

Retrieves all cost centre groups for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreGroupDtoListEnvelope**](CostCentreGroupDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centre_groups_count

> models::Int32Envelope get_cost_centre_groups_count(tenant_id, api_version, x_api_version)
Get the count of cost centre groups for a tenant

Retrieves the count of cost centre groups for the specified tenant using OData query options.

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


## get_cost_centres

> models::CostCentreDtoListEnvelope get_cost_centres(tenant_id, api_version, x_api_version)
Get all cost centres for a tenant

Retrieves all cost centres for the specified tenant using OData query options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CostCentreDtoListEnvelope**](CostCentreDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_cost_centres_count

> models::Int32Envelope get_cost_centres_count(tenant_id, api_version, x_api_version)
Get the count of cost centres for a tenant

Retrieves the count of cost centres for the specified tenant using OData query options.

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


## update_cost_centre

> models::EmptyEnvelope update_cost_centre(tenant_id, cost_centre_id, cost_centre_update_dto, api_version, x_api_version)
Update a cost centre

Updates an existing cost centre.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**cost_centre_id** | **uuid::Uuid** |  | [required] |
**cost_centre_update_dto** | [**CostCentreUpdateDto**](CostCentreUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cost_centre_budget

> models::EmptyEnvelope update_cost_centre_budget(tenant_id, budget_id, cost_centre_budget_update_dto, api_version, x_api_version)
Update a cost centre budget

Updates an existing cost centre budget.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**budget_id** | **uuid::Uuid** |  | [required] |
**cost_centre_budget_update_dto** | [**CostCentreBudgetUpdateDto**](CostCentreBudgetUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_cost_centre_group

> models::EmptyEnvelope update_cost_centre_group(tenant_id, group_id, cost_centre_group_update_dto, api_version, x_api_version)
Update a cost centre group

Updates an existing cost centre group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**group_id** | **uuid::Uuid** |  | [required] |
**cost_centre_group_update_dto** | [**CostCentreGroupUpdateDto**](CostCentreGroupUpdateDto.md) |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

