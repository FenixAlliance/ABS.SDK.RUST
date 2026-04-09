# \TeamContactEnrollmentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#create_tenant_team_contact_enrollment) | **POST** /api/v2/TenantsService/TeamContactEnrollments | Create a new tenant team contact enrollment
[**delete_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#delete_tenant_team_contact_enrollment) | **DELETE** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Delete a tenant team contact enrollment
[**get_tenant_team_contact_enrollment_by_id**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollment_by_id) | **GET** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Retrieve a single tenant team contact enrollment by its ID
[**get_tenant_team_contact_enrollments**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollments) | **GET** /api/v2/TenantsService/TeamContactEnrollments | Retrieve a list of tenant team contact enrollments
[**get_tenant_team_contact_enrollments_count**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollments_count) | **GET** /api/v2/TenantsService/TeamContactEnrollments/Count | Get the count of tenant team contact enrollments
[**update_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#update_tenant_team_contact_enrollment) | **PUT** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Update a tenant team contact enrollment



## create_tenant_team_contact_enrollment

> models::EmptyEnvelope create_tenant_team_contact_enrollment(tenant_id, api_version, x_api_version, tenant_team_contact_enrollment_create_dto)
Create a new tenant team contact enrollment

Create a new tenant team contact enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_team_contact_enrollment_create_dto** | Option<[**TenantTeamContactEnrollmentCreateDto**](TenantTeamContactEnrollmentCreateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tenant_team_contact_enrollment

> models::EmptyEnvelope delete_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, api_version, x_api_version)
Delete a tenant team contact enrollment

Delete a tenant team contact enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_contact_enrollment_id** | **uuid::Uuid** |  | [required] |
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


## get_tenant_team_contact_enrollment_by_id

> models::TenantTeamContactEnrollmentDtoEnvelope get_tenant_team_contact_enrollment_by_id(tenant_id, tenant_team_contact_enrollment_id, api_version, x_api_version)
Retrieve a single tenant team contact enrollment by its ID

Retrieve a single tenant team contact enrollment by its ID

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_contact_enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTeamContactEnrollmentDtoEnvelope**](TenantTeamContactEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_team_contact_enrollments

> models::TenantTeamContactEnrollmentDtoListEnvelope get_tenant_team_contact_enrollments(tenant_id, api_version, x_api_version)
Retrieve a list of tenant team contact enrollments

Retrieve a list of tenant team contact enrollments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::TenantTeamContactEnrollmentDtoListEnvelope**](TenantTeamContactEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tenant_team_contact_enrollments_count

> models::Int32Envelope get_tenant_team_contact_enrollments_count(tenant_id, api_version, x_api_version)
Get the count of tenant team contact enrollments

Get the count of tenant team contact enrollments

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


## update_tenant_team_contact_enrollment

> models::EmptyEnvelope update_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, api_version, x_api_version, tenant_team_contact_enrollment_update_dto)
Update a tenant team contact enrollment

Update a tenant team contact enrollment

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**tenant_team_contact_enrollment_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**tenant_team_contact_enrollment_update_dto** | Option<[**TenantTeamContactEnrollmentUpdateDto**](TenantTeamContactEnrollmentUpdateDto.md)> |  |  |

### Return type

[**models::EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

