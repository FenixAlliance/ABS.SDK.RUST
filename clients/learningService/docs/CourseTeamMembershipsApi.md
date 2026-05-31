# \CourseTeamMembershipsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_team_membership_async**](CourseTeamMembershipsApi.md#create_course_team_membership_async) | **POST** /api/v2/LearningService/CourseTeamMemberships | Create a course team membership
[**delete_course_team_membership_async**](CourseTeamMembershipsApi.md#delete_course_team_membership_async) | **DELETE** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Delete a course team membership
[**get_course_team_membership_by_id_async**](CourseTeamMembershipsApi.md#get_course_team_membership_by_id_async) | **GET** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Get course team membership by ID
[**get_course_team_memberships_async**](CourseTeamMembershipsApi.md#get_course_team_memberships_async) | **GET** /api/v2/LearningService/CourseTeamMemberships | Get all course team memberships
[**get_course_team_memberships_count_async**](CourseTeamMembershipsApi.md#get_course_team_memberships_count_async) | **GET** /api/v2/LearningService/CourseTeamMemberships/Count | Get course team memberships count
[**update_course_team_membership_async**](CourseTeamMembershipsApi.md#update_course_team_membership_async) | **PUT** /api/v2/LearningService/CourseTeamMemberships/{membershipId} | Update a course team membership



## create_course_team_membership_async

> create_course_team_membership_async(tenant_id, api_version, x_api_version, course_team_membership_create_dto)
Create a course team membership

Creates a new course team membership for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_team_membership_create_dto** | Option<[**CourseTeamMembershipCreateDto**](CourseTeamMembershipCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_team_membership_async

> delete_course_team_membership_async(tenant_id, membership_id, api_version, x_api_version)
Delete a course team membership

Deletes a course team membership by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**membership_id** | **String** |  | [required] |
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


## get_course_team_membership_by_id_async

> models::CourseTeamMembershipDto get_course_team_membership_by_id_async(membership_id, api_version, x_api_version)
Get course team membership by ID

Retrieves a specific course team membership by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**membership_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseTeamMembershipDto**](CourseTeamMembershipDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_team_memberships_async

> Vec<models::CourseTeamMembershipDto> get_course_team_memberships_async(tenant_id, api_version, x_api_version)
Get all course team memberships

Retrieves all course team memberships for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseTeamMembershipDto>**](CourseTeamMembershipDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_team_memberships_count_async

> i32 get_course_team_memberships_count_async(tenant_id, api_version, x_api_version)
Get course team memberships count

Returns the count of course team memberships for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

**i32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_course_team_membership_async

> update_course_team_membership_async(tenant_id, membership_id, api_version, x_api_version, course_team_membership_update_dto)
Update a course team membership

Updates an existing course team membership.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**membership_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_team_membership_update_dto** | Option<[**CourseTeamMembershipUpdateDto**](CourseTeamMembershipUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

