# \UserOptionsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_system_user_option**](UserOptionsApi.md#create_system_user_option) | **POST** /api/v2/SystemService/Users/{userId}/Options | Create a new user option (admin)
[**delete_system_user_option**](UserOptionsApi.md#delete_system_user_option) | **DELETE** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Delete a user option (admin)
[**get_system_user_option_by_id**](UserOptionsApi.md#get_system_user_option_by_id) | **GET** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Retrieve a single user option by its ID (admin)
[**get_system_user_options**](UserOptionsApi.md#get_system_user_options) | **GET** /api/v2/SystemService/Users/{userId}/Options | Retrieve a list of user options (admin)
[**get_system_user_options_count**](UserOptionsApi.md#get_system_user_options_count) | **GET** /api/v2/SystemService/Users/{userId}/Options/Count | Get the count of user options (admin)
[**update_system_user_option**](UserOptionsApi.md#update_system_user_option) | **PUT** /api/v2/SystemService/Users/{userId}/Options/{optionId} | Update a user option (admin)



## create_system_user_option

> models::EmptyEnvelope create_system_user_option(user_id, key, portal_id, api_version, x_api_version, option_create_dto)
Create a new user option (admin)

Admin endpoint to create an option for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## delete_system_user_option

> models::EmptyEnvelope delete_system_user_option(user_id, option_id, api_version, x_api_version)
Delete a user option (admin)

Admin endpoint to delete an option for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## get_system_user_option_by_id

> models::OptionDtoEnvelope get_system_user_option_by_id(user_id, option_id, api_version, x_api_version)
Retrieve a single user option by its ID (admin)

Admin endpoint to retrieve a single option for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## get_system_user_options

> models::OptionDtoListEnvelope get_system_user_options(user_id, portal_id, api_version, x_api_version)
Retrieve a list of user options (admin)

Admin endpoint to retrieve options for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## get_system_user_options_count

> models::Int32Envelope get_system_user_options_count(user_id, portal_id, api_version, x_api_version)
Get the count of user options (admin)

Admin endpoint to get the count of options for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## update_system_user_option

> models::EmptyEnvelope update_system_user_option(user_id, option_id, api_version, x_api_version, option_update_dto)
Update a user option (admin)

Admin endpoint to update an option for any user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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

