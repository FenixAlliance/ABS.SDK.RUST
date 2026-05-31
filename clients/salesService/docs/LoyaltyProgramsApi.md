# \LoyaltyProgramsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_loyalty_programs_async**](LoyaltyProgramsApi.md#count_loyalty_programs_async) | **GET** /api/v2/SalesService/LoyaltyPrograms/Count | Get loyalty programs count
[**create_loyalty_program_async**](LoyaltyProgramsApi.md#create_loyalty_program_async) | **POST** /api/v2/SalesService/LoyaltyPrograms | Create a loyalty program
[**delete_loyalty_program_async**](LoyaltyProgramsApi.md#delete_loyalty_program_async) | **DELETE** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Delete a loyalty program
[**get_loyalty_program_async**](LoyaltyProgramsApi.md#get_loyalty_program_async) | **GET** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Get loyalty program by ID
[**get_loyalty_programs_async**](LoyaltyProgramsApi.md#get_loyalty_programs_async) | **GET** /api/v2/SalesService/LoyaltyPrograms | Get loyalty programs
[**update_loyalty_program_async**](LoyaltyProgramsApi.md#update_loyalty_program_async) | **PUT** /api/v2/SalesService/LoyaltyPrograms/{loyaltyProgramId} | Update a loyalty program



## count_loyalty_programs_async

> models::Int32Envelope count_loyalty_programs_async(tenant_id)
Get loyalty programs count

Returns the total count of loyalty programs for the specified tenant with OData filter support.

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


## create_loyalty_program_async

> models::EmptyEnvelope create_loyalty_program_async(tenant_id, loyalty_program_create_dto)
Create a loyalty program

Creates a new loyalty program for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loyalty_program_create_dto** | Option<[**LoyaltyProgramCreateDto**](LoyaltyProgramCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_loyalty_program_async

> models::EmptyEnvelope delete_loyalty_program_async(tenant_id, loyalty_program_id)
Delete a loyalty program

Deletes an existing loyalty program by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loyalty_program_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loyalty_program_async

> models::LoyaltyProgramDtoEnvelope get_loyalty_program_async(tenant_id, loyalty_program_id)
Get loyalty program by ID

Retrieves a single loyalty program by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loyalty_program_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LoyaltyProgramDtoEnvelope**](LoyaltyProgramDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loyalty_programs_async

> models::LoyaltyProgramDtoListEnvelope get_loyalty_programs_async(tenant_id)
Get loyalty programs

Retrieves a list of loyalty programs for the specified tenant with OData query support.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |

### Return type

[**models::LoyaltyProgramDtoListEnvelope**](LoyaltyProgramDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_loyalty_program_async

> models::EmptyEnvelope update_loyalty_program_async(tenant_id, loyalty_program_id, loyalty_program_update_dto)
Update a loyalty program

Updates an existing loyalty program by its unique identifier.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**loyalty_program_id** | **uuid::Uuid** |  | [required] |
**loyalty_program_update_dto** | Option<[**LoyaltyProgramUpdateDto**](LoyaltyProgramUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

