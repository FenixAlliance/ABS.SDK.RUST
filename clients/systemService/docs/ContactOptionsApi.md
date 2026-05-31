# \ContactOptionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_system_contact_option**](ContactOptionsApi.md#create_system_contact_option) | **POST** /api/v2/SystemService/Contacts/{contactId}/Options | Create a new contact option (admin)
[**delete_system_contact_option**](ContactOptionsApi.md#delete_system_contact_option) | **DELETE** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Delete a contact option (admin)
[**get_system_contact_option_by_id**](ContactOptionsApi.md#get_system_contact_option_by_id) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Retrieve a single contact option by its ID (admin)
[**get_system_contact_options**](ContactOptionsApi.md#get_system_contact_options) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options | Retrieve a list of contact options (admin)
[**get_system_contact_options_count**](ContactOptionsApi.md#get_system_contact_options_count) | **GET** /api/v2/SystemService/Contacts/{contactId}/Options/Count | Get the count of contact options (admin)
[**update_system_contact_option**](ContactOptionsApi.md#update_system_contact_option) | **PUT** /api/v2/SystemService/Contacts/{contactId}/Options/{optionId} | Update a contact option (admin)



## create_system_contact_option

> models::EmptyEnvelope create_system_contact_option(contact_id, key, portal_id, api_version, x_api_version, option_create_dto)
Create a new contact option (admin)

Admin endpoint to create an option for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**key** | **String** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**option_create_dto** | Option<[**OptionCreateDto**](OptionCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_system_contact_option

> models::EmptyEnvelope delete_system_contact_option(contact_id, option_id, api_version, x_api_version)
Delete a contact option (admin)

Admin endpoint to delete an option for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
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


## get_system_contact_option_by_id

> models::OptionDtoEnvelope get_system_contact_option_by_id(contact_id, option_id, api_version, x_api_version)
Retrieve a single contact option by its ID (admin)

Admin endpoint to retrieve a single option for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OptionDtoEnvelope**](OptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_contact_options

> models::OptionDtoListEnvelope get_system_contact_options(contact_id, portal_id, api_version, x_api_version)
Retrieve a list of contact options (admin)

Admin endpoint to retrieve options for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::OptionDtoListEnvelope**](OptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_system_contact_options_count

> models::Int32Envelope get_system_contact_options_count(contact_id, portal_id, api_version, x_api_version)
Get the count of contact options (admin)

Admin endpoint to get the count of options for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**portal_id** | Option<**uuid::Uuid**> |  |  |
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


## update_system_contact_option

> models::EmptyEnvelope update_system_contact_option(contact_id, option_id, api_version, x_api_version, option_update_dto)
Update a contact option (admin)

Admin endpoint to update an option for any contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**option_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**option_update_dto** | Option<[**OptionUpdateDto**](OptionUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

