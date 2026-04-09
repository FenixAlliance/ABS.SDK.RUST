# \UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_current_user_followers_async**](UsersApi.md#count_current_user_followers_async) | **GET** /api/v2/Me/Followers/Count | Count the social profiles that follow the current user
[**count_current_user_follows_async**](UsersApi.md#count_current_user_follows_async) | **GET** /api/v2/Me/Follows/Count | Count the social profiles that the current user follows
[**count_current_user_notifications_async**](UsersApi.md#count_current_user_notifications_async) | **GET** /api/v2/Me/Notifications/Count | Count the notifications for the current user
[**count_current_user_tenants_async**](UsersApi.md#count_current_user_tenants_async) | **GET** /api/v2/Me/Tenants/Count | Count the tenants that the current user is enrolled in
[**get_current_user_addresses_async**](UsersApi.md#get_current_user_addresses_async) | **GET** /api/v2/Me/Addresses | Get the list of addresses for the current user
[**get_current_user_async**](UsersApi.md#get_current_user_async) | **GET** /api/v2/Me | Gets the current user
[**get_current_user_avatar_async**](UsersApi.md#get_current_user_avatar_async) | **GET** /api/v2/Me/Avatar | Get the current user's avatar
[**get_current_user_cart_async**](UsersApi.md#get_current_user_cart_async) | **GET** /api/v2/Me/Cart | Get the current user's cart
[**get_current_user_enrollments_async**](UsersApi.md#get_current_user_enrollments_async) | **GET** /api/v2/Me/Enrollments | Get the list of enrollments for the current user
[**get_current_user_enrollments_extended_async**](UsersApi.md#get_current_user_enrollments_extended_async) | **GET** /api/v2/Me/Enrollments/Extended | Get the list of enrollments for the current user
[**get_current_user_followers_async**](UsersApi.md#get_current_user_followers_async) | **GET** /api/v2/Me/Followers | Get the social profiles that follow the current user
[**get_current_user_follows_async**](UsersApi.md#get_current_user_follows_async) | **GET** /api/v2/Me/Follows | Get the social profiles that the current user follows
[**get_current_user_invitation_async**](UsersApi.md#get_current_user_invitation_async) | **GET** /api/v2/Me/Invitations | Get the list of tenant enrollment invitations for the current user
[**get_current_user_notifications_async**](UsersApi.md#get_current_user_notifications_async) | **GET** /api/v2/Me/Notifications | Get the list of notifications for the current user
[**get_current_user_settings_async**](UsersApi.md#get_current_user_settings_async) | **GET** /api/v2/Me/Settings | Get the settings for the current user
[**get_current_user_social_profile_async**](UsersApi.md#get_current_user_social_profile_async) | **GET** /api/v2/Me/SocialProfile | Get the current user's social profile
[**get_current_user_tenants_async**](UsersApi.md#get_current_user_tenants_async) | **GET** /api/v2/Me/Tenants | Get the tenants that the current user is enrolled in
[**get_current_user_tenants_extended_async**](UsersApi.md#get_current_user_tenants_extended_async) | **GET** /api/v2/Me/Tenants/Extended | Get the tenants that the current user is enrolled in
[**get_current_user_wallet_async**](UsersApi.md#get_current_user_wallet_async) | **GET** /api/v2/Me/Wallet | Get the current user's billing profile
[**get_enrollment_async**](UsersApi.md#get_enrollment_async) | **GET** /api/v2/Me/Enrollments/{enrollmentId} | Get a single TenantEnrollment by its ID
[**get_extended_current_user_async**](UsersApi.md#get_extended_current_user_async) | **GET** /api/v2/Me/Extended | Get the current user's extended profile
[**patch_current_user_async**](UsersApi.md#patch_current_user_async) | **PATCH** /api/v2/Me | Partially update the current user's profile
[**update_avatar_async**](UsersApi.md#update_avatar_async) | **POST** /api/v2/Me/Avatar | Update the current user's avatar
[**update_current_user_async**](UsersApi.md#update_current_user_async) | **PUT** /api/v2/Me | Update the current user's profile
[**update_current_user_settings_async**](UsersApi.md#update_current_user_settings_async) | **PUT** /api/v2/Me/Settings | Update the settings for the current user



## count_current_user_followers_async

> models::Int32Envelope count_current_user_followers_async(api_version, x_api_version)
Count the social profiles that follow the current user

Count the social profiles that follow the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_current_user_follows_async

> models::Int32Envelope count_current_user_follows_async(api_version, x_api_version)
Count the social profiles that the current user follows

Count the social profiles that the current user follows

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_current_user_notifications_async

> models::Int32Envelope count_current_user_notifications_async(api_version, x_api_version)
Count the notifications for the current user

Count the notifications for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## count_current_user_tenants_async

> models::Int32Envelope count_current_user_tenants_async(api_version, x_api_version)
Count the tenants that the current user is enrolled in

Count the tenants that the current user is enrolled in

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_addresses_async

> models::AddressDtoListEnvelope get_current_user_addresses_async(api_version, x_api_version)
Get the list of addresses for the current user

Get the list of addresses for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::AddressDtoListEnvelope**](AddressDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_async

> models::UserDtoEnvelope get_current_user_async(api_version, x_api_version)
Gets the current user

Get the currently acting user.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserDtoEnvelope**](UserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_avatar_async

> std::path::PathBuf get_current_user_avatar_async(api_version, x_api_version)
Get the current user's avatar

Get the current user's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_cart_async

> models::CartDtoEnvelope get_current_user_cart_async(api_version, x_api_version)
Get the current user's cart

Get the current user's cart

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_enrollments_async

> models::TenantEnrollmentDtoListEnvelope get_current_user_enrollments_async(api_version, x_api_version)
Get the list of enrollments for the current user

Get the list of enrollments for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_enrollments_extended_async

> models::ExtendedTenantEnrollmentDtoListEnvelope get_current_user_enrollments_extended_async(api_version, x_api_version)
Get the list of enrollments for the current user

Get the list of enrollments for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedTenantEnrollmentDtoListEnvelope**](ExtendedTenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_followers_async

> models::FollowRecordDtoListEnvelope get_current_user_followers_async(api_version, x_api_version)
Get the social profiles that follow the current user

Get the social profiles that follow the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_follows_async

> models::FollowRecordDtoListEnvelope get_current_user_follows_async(api_version, x_api_version)
Get the social profiles that the current user follows

Get the social profiles that the current user follows

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::FollowRecordDtoListEnvelope**](FollowRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_invitation_async

> models::TenantInvitationDtoListEnvelope get_current_user_invitation_async(api_version, x_api_version)
Get the list of tenant enrollment invitations for the current user

Get the list of tenant enrollment invitations for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_notifications_async

> models::NotificationDtoListEnvelope get_current_user_notifications_async(api_version, x_api_version)
Get the list of notifications for the current user

Get the list of notifications for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::NotificationDtoListEnvelope**](NotificationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_settings_async

> models::UserSettingsDtoEnvelope get_current_user_settings_async(api_version, x_api_version)
Get the settings for the current user

Get the settings for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::UserSettingsDtoEnvelope**](UserSettingsDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_social_profile_async

> models::SocialProfileDtoEnvelope get_current_user_social_profile_async(api_version, x_api_version)
Get the current user's social profile

Get the current user's social profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_tenants_async

> models::TenantDtoListEnvelope get_current_user_tenants_async(api_version, x_api_version)
Get the tenants that the current user is enrolled in

Get the tenants that the current user is enrolled in

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantDtoListEnvelope**](TenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_tenants_extended_async

> models::ExtendedTenantDtoListEnvelope get_current_user_tenants_extended_async(api_version, x_api_version)
Get the tenants that the current user is enrolled in

Get the tenants that the current user is enrolled in

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedTenantDtoListEnvelope**](ExtendedTenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_current_user_wallet_async

> models::WalletDtoEnvelope get_current_user_wallet_async(api_version, x_api_version)
Get the current user's billing profile

Get the current user's billing profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_enrollment_async

> models::TenantEnrollmentDtoEnvelope get_enrollment_async(enrollment_id, api_version, x_api_version)
Get a single TenantEnrollment by its ID

Get a single TenantEnrollment by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantEnrollmentDtoEnvelope**](TenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_current_user_async

> models::ExtendedUserDtoEnvelope get_extended_current_user_async(api_version, x_api_version)
Get the current user's extended profile

Get the current user's extended profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedUserDtoEnvelope**](ExtendedUserDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_current_user_async

> models::EmptyEnvelope patch_current_user_async(api_version, x_api_version, operation)
Partially update the current user's profile

Partially update the current user's profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_avatar_async

> models::EmptyEnvelope update_avatar_async(api_version, x_api_version, avatar)
Update the current user's avatar

Update the current user's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**avatar** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_current_user_async

> models::EmptyEnvelope update_current_user_async(api_version, x_api_version, user_update_dto)
Update the current user's profile

Update the current user's profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_update_dto** | Option<[**UserUpdateDto**](UserUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_current_user_settings_async

> models::UserSettingsDtoEnvelope update_current_user_settings_async(api_version, x_api_version, user_settings_update_dto)
Update the settings for the current user

Update the settings for the current user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**user_settings_update_dto** | Option<[**UserSettingsUpdateDto**](UserSettingsUpdateDto.md)> |  |  |

### Return type

[**models::UserSettingsDtoEnvelope**](UserSettingsDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml, multipart/form-data
- **Accept**: application/json, application/xml, multipart/form-data

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

