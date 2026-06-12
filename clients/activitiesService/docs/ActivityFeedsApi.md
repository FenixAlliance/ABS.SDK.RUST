# \ActivityFeedsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_activity_types_async**](ActivityFeedsApi.md#count_activity_types_async) | **GET** /api/v2/ActivitiesService/ActivityTypes/Count | Count Activity Types
[**create_activity_async**](ActivityFeedsApi.md#create_activity_async) | **POST** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities | Create an activity
[**create_activity_type_async**](ActivityFeedsApi.md#create_activity_type_async) | **POST** /api/v2/ActivitiesService/ActivityTypes | Create Activity Type
[**delete_activity_async**](ActivityFeedsApi.md#delete_activity_async) | **DELETE** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Delete an activity
[**delete_activity_type_async**](ActivityFeedsApi.md#delete_activity_type_async) | **DELETE** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Delete Activity Type
[**get_activities_async**](ActivityFeedsApi.md#get_activities_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities | Get activities
[**get_activities_count_async**](ActivityFeedsApi.md#get_activities_count_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/Count | Count activities
[**get_activity_async**](ActivityFeedsApi.md#get_activity_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Get activity by ID
[**get_activity_feed_async**](ActivityFeedsApi.md#get_activity_feed_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId} | Get activity feed by ID
[**get_activity_feeds_async**](ActivityFeedsApi.md#get_activity_feeds_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds | Get activity feeds
[**get_activity_feeds_count_async**](ActivityFeedsApi.md#get_activity_feeds_count_async) | **GET** /api/v2/ActivitiesService/ActivityFeeds/Count | Count activity feeds
[**get_activity_type_by_id_async**](ActivityFeedsApi.md#get_activity_type_by_id_async) | **GET** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Get Activity Type
[**get_activity_types_async**](ActivityFeedsApi.md#get_activity_types_async) | **GET** /api/v2/ActivitiesService/ActivityTypes | Get Activity Types
[**patch_activity_async**](ActivityFeedsApi.md#patch_activity_async) | **PATCH** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Patch an activity
[**patch_activity_type_async**](ActivityFeedsApi.md#patch_activity_type_async) | **PATCH** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Patch Activity Type
[**update_activity_async**](ActivityFeedsApi.md#update_activity_async) | **PUT** /api/v2/ActivitiesService/ActivityFeeds/{activityFeedId}/Activities/{activityId} | Update an activity
[**update_activity_type_async**](ActivityFeedsApi.md#update_activity_type_async) | **PUT** /api/v2/ActivitiesService/ActivityTypes/{activityTypeId} | Update Activity Type



## count_activity_types_async

> models::Int32Envelope count_activity_types_async(tenant_id, api_version, x_api_version)
Count Activity Types

Count activity types for the current tenant.

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


## create_activity_async

> models::ActivityRecordDtoEnvelope create_activity_async(tenant_id, activity_feed_id, api_version, x_api_version, activity_record_create_dto)
Create an activity

Creates a new activity in a specific activity feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**activity_record_create_dto** | Option<[**ActivityRecordCreateDto**](ActivityRecordCreateDto.md)> |  |  |

### Return type

[**models::ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_activity_type_async

> models::Envelope create_activity_type_async(tenant_id, api_version, x_api_version, activity_type_create_dto)
Create Activity Type

Create a new activity type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**activity_type_create_dto** | Option<[**ActivityTypeCreateDto**](ActivityTypeCreateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_activity_async

> models::EmptyEnvelope delete_activity_async(tenant_id, activity_feed_id, activity_id, api_version, x_api_version)
Delete an activity

Deletes an activity from an activity feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**activity_id** | **uuid::Uuid** |  | [required] |
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


## delete_activity_type_async

> models::Envelope delete_activity_type_async(tenant_id, activity_type_id, api_version, x_api_version)
Delete Activity Type

Delete an activity type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activities_async

> models::ActivityRecordDtoListEnvelope get_activities_async(tenant_id, activity_feed_id, api_version, x_api_version)
Get activities

Retrieves activities for a specific activity feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityRecordDtoListEnvelope**](ActivityRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activities_count_async

> models::Int32Envelope get_activities_count_async(tenant_id, activity_feed_id, api_version, x_api_version)
Count activities

Returns the count of activities for a specific activity feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
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


## get_activity_async

> models::ActivityRecordDtoEnvelope get_activity_async(tenant_id, activity_feed_id, activity_id, api_version, x_api_version)
Get activity by ID

Retrieves a specific activity by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**activity_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activity_feed_async

> models::ActivityFeedDtoEnvelope get_activity_feed_async(tenant_id, activity_feed_id, api_version, x_api_version)
Get activity feed by ID

Retrieves a specific activity feed by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityFeedDtoEnvelope**](ActivityFeedDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activity_feeds_async

> models::ActivityFeedDtoListEnvelope get_activity_feeds_async(tenant_id, api_version, x_api_version)
Get activity feeds

Retrieves a list of activity feeds for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityFeedDtoListEnvelope**](ActivityFeedDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activity_feeds_count_async

> models::Int32Envelope get_activity_feeds_count_async(tenant_id, api_version, x_api_version)
Count activity feeds

Returns the count of activity feeds for the specified tenant.

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


## get_activity_type_by_id_async

> models::ActivityTypeDtoEnvelope get_activity_type_by_id_async(tenant_id, activity_type_id, api_version, x_api_version)
Get Activity Type

Get an activity type by ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityTypeDtoEnvelope**](ActivityTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_activity_types_async

> models::ActivityTypeDtoListEnvelope get_activity_types_async(tenant_id, api_version, x_api_version)
Get Activity Types

Get a list of activity types for the current tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::ActivityTypeDtoListEnvelope**](ActivityTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## patch_activity_async

> models::EmptyEnvelope patch_activity_async(tenant_id, activity_feed_id, activity_id, api_version, x_api_version, operation)
Patch an activity

Patch an activity

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**activity_id** | **uuid::Uuid** |  | [required] |
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


## patch_activity_type_async

> models::EmptyEnvelope patch_activity_type_async(tenant_id, activity_type_id, api_version, x_api_version, operation)
Patch Activity Type

Patch an activity type

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_type_id** | **uuid::Uuid** |  | [required] |
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


## update_activity_async

> models::ActivityRecordDtoEnvelope update_activity_async(tenant_id, activity_feed_id, activity_id, api_version, x_api_version, activity_record_update_dto)
Update an activity

Updates an existing activity.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_feed_id** | **uuid::Uuid** |  | [required] |
**activity_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**activity_record_update_dto** | Option<[**ActivityRecordUpdateDto**](ActivityRecordUpdateDto.md)> |  |  |

### Return type

[**models::ActivityRecordDtoEnvelope**](ActivityRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_activity_type_async

> models::Envelope update_activity_type_async(tenant_id, activity_type_id, api_version, x_api_version, activity_type_update_dto)
Update Activity Type

Update an existing activity type.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**activity_type_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**activity_type_update_dto** | Option<[**ActivityTypeUpdateDto**](ActivityTypeUpdateDto.md)> |  |  |

### Return type

[**models::Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

