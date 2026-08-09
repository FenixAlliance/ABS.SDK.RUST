# \UsersApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**admin_preview_user_email_template**](UsersApi.md#admin_preview_user_email_template) | **POST** /api/v2/SystemService/Users/{userId}/Emails/Preview | Preview the rendered email for a user.
[**admin_send_user_email**](UsersApi.md#admin_send_user_email) | **POST** /api/v2/SystemService/Users/{userId}/Emails/Send | Send an email to a user.
[**create_account_holder_async**](UsersApi.md#create_account_holder_async) | **POST** /api/v2/SystemService/Users | Create a new user
[**delete_account_holder_async**](UsersApi.md#delete_account_holder_async) | **DELETE** /api/v2/SystemService/Users/{userId} | Delete a user
[**get_extended_account_holder_async**](UsersApi.md#get_extended_account_holder_async) | **GET** /api/v2/SystemService/Users/{userId}/Extended | Retrieve an extended user by ID
[**get_extended_users_async**](UsersApi.md#get_extended_users_async) | **GET** /api/v2/SystemService/Users/Extended | Retrieve a list of extended users
[**get_extended_users_count_async**](UsersApi.md#get_extended_users_count_async) | **GET** /api/v2/SystemService/Users/Extended/Count | Get the count of extended users
[**get_user_admin_detail_async**](UsersApi.md#get_user_admin_detail_async) | **GET** /api/v2/SystemService/Users/{userId}/AdminDetail | Retrieve the admin detail aggregate for a user
[**get_user_async**](UsersApi.md#get_user_async) | **GET** /api/v2/SystemService/Users/{userId} | Retrieve a user by ID
[**get_users_async**](UsersApi.md#get_users_async) | **GET** /api/v2/SystemService/Users | Retrieve a list of users
[**get_users_count_async**](UsersApi.md#get_users_count_async) | **GET** /api/v2/SystemService/Users/Count | Get the count of users
[**patch_account_holder_async**](UsersApi.md#patch_account_holder_async) | **PATCH** /api/v2/SystemService/Users/{userId} | Partially update a user
[**set_user_password_async**](UsersApi.md#set_user_password_async) | **POST** /api/v2/SystemService/Users/{userId}/Password | Set a user's password
[**update_account_holder_admin_profile_async**](UsersApi.md#update_account_holder_admin_profile_async) | **PUT** /api/v2/SystemService/Users/{userId}/AdminProfile | Update a user's admin-managed profile
[**update_account_holder_async**](UsersApi.md#update_account_holder_async) | **PUT** /api/v2/SystemService/Users/{userId} | Update a user



## admin_preview_user_email_template

> admin_preview_user_email_template(user_id, api_version, x_api_version, email_dispatch_request)
Preview the rendered email for a user.

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## admin_send_user_email

> models::EmptyEnvelope admin_send_user_email(user_id, api_version, x_api_version, email_dispatch_request)
Send an email to a user.

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_account_holder_async

> models::EmptyEnvelope create_account_holder_async(api_version, x_api_version, user_create_dto)
Create a new user

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_create_dto** | Option<[**UserCreateDto**](UserCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_account_holder_async

> models::EmptyEnvelope delete_account_holder_async(user_id, api_version, x_api_version)
Delete a user

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
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


## get_extended_account_holder_async

> models::ExtendedUserDtoEnvelope get_extended_account_holder_async(user_id, api_version, x_api_version)
Retrieve an extended user by ID

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedUserDtoEnvelope**](ExtendedUserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_users_async

> models::ExtendedUserDtoListEnvelope get_extended_users_async(api_version, x_api_version, extended_user_dto_collection_query_parameters)
Retrieve a list of extended users

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**extended_user_dto_collection_query_parameters** | Option<[**ExtendedUserDtoCollectionQueryParameters**](ExtendedUserDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::ExtendedUserDtoListEnvelope**](ExtendedUserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_users_count_async

> models::Int32Envelope get_extended_users_count_async(api_version, x_api_version, extended_user_dto_collection_query_parameters)
Get the count of extended users

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**extended_user_dto_collection_query_parameters** | Option<[**ExtendedUserDtoCollectionQueryParameters**](ExtendedUserDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_user_admin_detail_async

> models::UserAdminDetailDtoEnvelope get_user_admin_detail_async(user_id, tenant_id, api_version, x_api_version)
Retrieve the admin detail aggregate for a user

Returns the user's orders, external logins, and — for the supplied tenant — the enrollment with its granted roles/permissions and the tenant role/permission catalogs. Global administrators only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **String** |  | [required] |
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserAdminDetailDtoEnvelope**](UserAdminDetailDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_user_async

> models::UserDtoEnvelope get_user_async(user_id, api_version, x_api_version)
Retrieve a user by ID

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserDtoEnvelope**](UserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_users_async

> models::UserDtoListEnvelope get_users_async(api_version, x_api_version, user_dto_collection_query_parameters)
Retrieve a list of users

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_dto_collection_query_parameters** | Option<[**UserDtoCollectionQueryParameters**](UserDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::UserDtoListEnvelope**](UserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_users_count_async

> models::Int32Envelope get_users_count_async(api_version, x_api_version, user_dto_collection_query_parameters)
Get the count of users

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_dto_collection_query_parameters** | Option<[**UserDtoCollectionQueryParameters**](UserDtoCollectionQueryParameters.md)> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_account_holder_async

> models::EmptyEnvelope patch_account_holder_async(user_id, api_version, x_api_version, patch_operation)
Partially update a user

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**patch_operation** | Option<[**Vec<models::PatchOperation>**](PatchOperation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_user_password_async

> models::EmptyEnvelope set_user_password_async(user_id, api_version, x_api_version, set_user_password_dto)
Set a user's password

Replaces the user's password with the supplied value. Global administrators only.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**set_user_password_dto** | Option<[**SetUserPasswordDto**](SetUserPasswordDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_holder_admin_profile_async

> models::EmptyEnvelope update_account_holder_admin_profile_async(user_id, api_version, x_api_version, user_admin_update_dto)
Update a user's admin-managed profile

Updates the identity fields (email/username, re-normalized by Identity) and display fields a global administrator may change on a user, and toggles two-factor and lockout. Normalized email/username and the access-failed count are never accepted. This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_admin_update_dto** | Option<[**UserAdminUpdateDto**](UserAdminUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_account_holder_async

> models::EmptyEnvelope update_account_holder_async(user_id, api_version, x_api_version, user_update_dto)
Update a user

This action is only available for global administrators.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_update_dto** | Option<[**UserUpdateDto**](UserUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

