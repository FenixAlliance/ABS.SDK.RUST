# \ContactsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_contact_async**](ContactsApi.md#create_contact_async) | **POST** /api/v2/CrmService/Contacts | Create a new contact
[**delete_contact_async**](ContactsApi.md#delete_contact_async) | **DELETE** /api/v2/CrmService/Contacts/{contactId} | Delete a contact
[**get_business_owned_individual_async**](ContactsApi.md#get_business_owned_individual_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId} | Get a Contact of type Individual by ID
[**get_business_owned_individuals_async**](ContactsApi.md#get_business_owned_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals | Get all contacts of type individual
[**get_business_owned_individuals_count_async**](ContactsApi.md#get_business_owned_individuals_count_async) | **GET** /api/v2/CrmService/Contacts/Individuals/Count | Get all contacts of type individual count
[**get_business_owned_organization_async**](ContactsApi.md#get_business_owned_organization_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId} | Get a Contact of type Organization by ID
[**get_business_owned_organizations_async**](ContactsApi.md#get_business_owned_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations | Get all contacts of type organization
[**get_business_owned_organizations_count_async**](ContactsApi.md#get_business_owned_organizations_count_async) | **GET** /api/v2/CrmService/Contacts/Organizations/Count | Get all contacts of type organization count
[**get_contact_async**](ContactsApi.md#get_contact_async) | **GET** /api/v2/CrmService/Contacts/{contactId} | Get a contact by ID
[**get_contact_avatar_async**](ContactsApi.md#get_contact_avatar_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Avatar | Get a contact's avatar
[**get_contact_cart_async**](ContactsApi.md#get_contact_cart_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Cart | Get a contact's cart
[**get_contact_profiles_async**](ContactsApi.md#get_contact_profiles_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Profiles | Get a contact's social profiles
[**get_contact_social_profile_async**](ContactsApi.md#get_contact_social_profile_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/SocialProfile | Get a contact's social profile
[**get_contact_wallet_async**](ContactsApi.md#get_contact_wallet_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Wallet | Get a contact's wallet
[**get_contacts_async**](ContactsApi.md#get_contacts_async) | **GET** /api/v2/CrmService/Contacts | Get all business owned contacts
[**get_contacts_count_async**](ContactsApi.md#get_contacts_count_async) | **GET** /api/v2/CrmService/Contacts/Count | Get all business owned contacts count
[**get_extended_business_owned_individuals_async**](ContactsApi.md#get_extended_business_owned_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals/Extended | Get all contacts of type individual
[**get_extended_business_owned_organizations_async**](ContactsApi.md#get_extended_business_owned_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations/Extended | Get all contacts of type organization
[**get_extended_contact_async**](ContactsApi.md#get_extended_contact_async) | **GET** /api/v2/CrmService/Contacts/{contactId}/Extended | Get a contact by ID
[**get_extended_contacts_async**](ContactsApi.md#get_extended_contacts_async) | **GET** /api/v2/CrmService/Contacts/Extended | Get all business owned contacts
[**get_individual_related_individuals_async**](ContactsApi.md#get_individual_related_individuals_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId}/Individuals | Get individual related individuals
[**get_individual_related_organizations_async**](ContactsApi.md#get_individual_related_organizations_async) | **GET** /api/v2/CrmService/Contacts/Individuals/{contactId}/Organizations | Get individual related organizations
[**get_organization_related_individuals_async**](ContactsApi.md#get_organization_related_individuals_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId}/Individuals | Get organization related individuals
[**get_organization_related_organizations_async**](ContactsApi.md#get_organization_related_organizations_async) | **GET** /api/v2/CrmService/Contacts/Organizations/{contactId}/Organizations | Get organization related organizations
[**patch_contact_async**](ContactsApi.md#patch_contact_async) | **PATCH** /api/v2/CrmService/Contacts/{contactId} | Patch a contact
[**preview_contact_email_template**](ContactsApi.md#preview_contact_email_template) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/Preview | Preview the rendered email for a contact.
[**send_contact_email**](ContactsApi.md#send_contact_email) | **POST** /api/v2/CrmService/Contacts/{contactId}/Emails/Send | Send an email to a contact.
[**update_contact_async**](ContactsApi.md#update_contact_async) | **PUT** /api/v2/CrmService/Contacts/{contactId} | Update a contact
[**update_contact_avatar_async**](ContactsApi.md#update_contact_avatar_async) | **POST** /api/v2/CrmService/Contacts/{contactId}/Avatar | Update a contact's avatar
[**upsert_tenant_onto_another_tenant_contact_list_async**](ContactsApi.md#upsert_tenant_onto_another_tenant_contact_list_async) | **POST** /api/v2/CrmService/Contacts/Organizations/Upsert | Upsert a tenant onto another tenant's contact list
[**upsert_user_onto_another_tenant_contact_list_async**](ContactsApi.md#upsert_user_onto_another_tenant_contact_list_async) | **POST** /api/v2/CrmService/Contacts/Individuals/Upsert | Upsert a user onto a tenant's contact list



## create_contact_async

> models::EmptyEnvelope create_contact_async(tenant_id, api_version, x_api_version, contact_create_dto)
Create a new contact

Create a new contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_create_dto** | Option<[**ContactCreateDto**](ContactCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_async

> models::EmptyEnvelope delete_contact_async(tenant_id, contact_id, api_version, x_api_version)
Delete a contact

Delete a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
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


## get_business_owned_individual_async

> models::ContactDtoEnvelope get_business_owned_individual_async(tenant_id, contact_id, api_version, x_api_version)
Get a Contact of type Individual by ID

Get a Contact of type Individual by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_owned_individuals_async

> models::ContactDtoListEnvelope get_business_owned_individuals_async(tenant_id, api_version, x_api_version)
Get all contacts of type individual

Get all contacts of type individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_owned_individuals_count_async

> models::ContactDtoListEnvelope get_business_owned_individuals_count_async(tenant_id, api_version, x_api_version)
Get all contacts of type individual count

Get all contacts of type individual count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_owned_organization_async

> models::ContactDtoEnvelope get_business_owned_organization_async(tenant_id, contact_id, api_version, x_api_version)
Get a Contact of type Organization by ID

Get a Contact of type Organization by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_owned_organizations_async

> Vec<models::ContactDto> get_business_owned_organizations_async(tenant_id, api_version, x_api_version)
Get all contacts of type organization

Get all contacts of type organization

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::ContactDto>**](ContactDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_business_owned_organizations_count_async

> models::ContactDtoListEnvelope get_business_owned_organizations_count_async(tenant_id, api_version, x_api_version)
Get all contacts of type organization count

Get all contacts of type organization count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_async

> models::ContactDtoEnvelope get_contact_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact by ID

Get a contact by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_avatar_async

> models::EmptyEnvelope get_contact_avatar_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact's avatar

Get a contact's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
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


## get_contact_cart_async

> models::CartDtoEnvelope get_contact_cart_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact's cart

Get a contact's cart

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_profiles_async

> models::ContactProfileDtoListEnvelope get_contact_profiles_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact's social profiles

Get a contact's social profiles

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactProfileDtoListEnvelope**](ContactProfileDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_social_profile_async

> models::SocialProfileDtoEnvelope get_contact_social_profile_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact's social profile

Get a contact's social profile

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_wallet_async

> models::WalletDtoEnvelope get_contact_wallet_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact's wallet

Get a contact's wallet

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contacts_async

> models::ContactDtoListEnvelope get_contacts_async(tenant_id, api_version, x_api_version)
Get all business owned contacts

Get all business owned contacts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contacts_count_async

> models::ContactDtoListEnvelope get_contacts_count_async(tenant_id, api_version, x_api_version)
Get all business owned contacts count

Get all business owned contacts count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_business_owned_individuals_async

> models::ExtendedContactDtoListEnvelope get_extended_business_owned_individuals_async(tenant_id, api_version, x_api_version)
Get all contacts of type individual

Get all contacts of type individual

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_business_owned_organizations_async

> models::ExtendedContactDtoListEnvelope get_extended_business_owned_organizations_async(tenant_id, api_version, x_api_version)
Get all contacts of type organization

Get all contacts of type organization

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_contact_async

> models::ExtendedContactDtoEnvelope get_extended_contact_async(tenant_id, contact_id, api_version, x_api_version)
Get a contact by ID

Get a contact by ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedContactDtoEnvelope**](ExtendedContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_extended_contacts_async

> models::ExtendedContactDtoListEnvelope get_extended_contacts_async(tenant_id, api_version, x_api_version)
Get all business owned contacts

Get all business owned contacts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ExtendedContactDtoListEnvelope**](ExtendedContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_individual_related_individuals_async

> models::ContactDtoListEnvelope get_individual_related_individuals_async(tenant_id, contact_id, api_version, x_api_version)
Get individual related individuals

Get individual related individuals

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_individual_related_organizations_async

> models::ContactDtoListEnvelope get_individual_related_organizations_async(tenant_id, contact_id, api_version, x_api_version)
Get individual related organizations

Get individual related organizations

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_organization_related_individuals_async

> models::ContactDtoListEnvelope get_organization_related_individuals_async(tenant_id, contact_id, api_version, x_api_version)
Get organization related individuals

Get organization related individuals

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_organization_related_organizations_async

> models::ContactDtoListEnvelope get_organization_related_organizations_async(tenant_id, contact_id, api_version, x_api_version)
Get organization related organizations

Get organization related organizations

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoListEnvelope**](ContactDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_contact_async

> models::EmptyEnvelope patch_contact_async(tenant_id, contact_id, api_version, x_api_version, operation)
Patch a contact

Patch a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**operation** | Option<[**Vec<models::Operation>**](Operation.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## preview_contact_email_template

> preview_contact_email_template(contact_id, api_version, x_api_version, email_dispatch_request)
Preview the rendered email for a contact.

This action is only available for global administrators (business_owner role).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_contact_email

> send_contact_email(contact_id, api_version, x_api_version, email_dispatch_request)
Send an email to a contact.

This action is only available for global administrators (business_owner role).

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**email_dispatch_request** | Option<[**EmailDispatchRequest**](EmailDispatchRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_contact_async

> models::EmptyEnvelope update_contact_async(tenant_id, contact_id, api_version, x_api_version, contact_update_dto)
Update a contact

Update a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**contact_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**contact_update_dto** | Option<[**ContactUpdateDto**](ContactUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_contact_avatar_async

> models::EmptyEnvelope update_contact_avatar_async(contact_id, tenant_id, api_version, x_api_version, avatar)
Update a contact's avatar

Update a contact's avatar

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**contact_id** | **uuid::Uuid** |  | [required] |
**tenant_id** | Option<**uuid::Uuid**> |  |  |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**avatar** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upsert_tenant_onto_another_tenant_contact_list_async

> models::ContactDtoEnvelope upsert_tenant_onto_another_tenant_contact_list_async(tenant_id, related_tenant_id, api_version, x_api_version)
Upsert a tenant onto another tenant's contact list

Upsert a tenant onto another tenant's contact list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**related_tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upsert_user_onto_another_tenant_contact_list_async

> models::ContactDtoEnvelope upsert_user_onto_another_tenant_contact_list_async(tenant_id, related_user_id, api_version, x_api_version)
Upsert a user onto a tenant's contact list

Upsert a user onto a tenant's contact list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**related_user_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ContactDtoEnvelope**](ContactDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

