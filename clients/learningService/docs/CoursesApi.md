# \CoursesApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_async**](CoursesApi.md#create_course_async) | **POST** /api/v2/LearningService/Courses | Create a new course
[**delete_course_async**](CoursesApi.md#delete_course_async) | **DELETE** /api/v2/LearningService/Courses/{courseId} | Delete a course
[**get_course_articles_by_course_wiki_async**](CoursesApi.md#get_course_articles_by_course_wiki_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Articles/{wikiId} | Get course articles by course wiki
[**get_course_articles_by_course_wiki_count_async**](CoursesApi.md#get_course_articles_by_course_wiki_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Articles/{wikiId}/Count | Get course articles by course wiki count
[**get_course_assignments_by_course_async**](CoursesApi.md#get_course_assignments_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Assignments | Get course assignments by course
[**get_course_assignments_by_course_count_async**](CoursesApi.md#get_course_assignments_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Assignments/Count | Get course assignments by course count
[**get_course_by_id_async**](CoursesApi.md#get_course_by_id_async) | **GET** /api/v2/LearningService/Courses/{courseId} | Get course by ID
[**get_course_categories_by_course_async**](CoursesApi.md#get_course_categories_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Categories | Get course categories by course
[**get_course_categories_by_course_count_async**](CoursesApi.md#get_course_categories_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Categories/Count | Get course categories by course count
[**get_course_cohorts_by_course_async**](CoursesApi.md#get_course_cohorts_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Cohorts | Get course cohorts by course
[**get_course_cohorts_by_course_count_async**](CoursesApi.md#get_course_cohorts_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Cohorts/Count | Get course cohorts by course count
[**get_course_enrollments_by_course_async**](CoursesApi.md#get_course_enrollments_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Enrollments | Get enrollments by course
[**get_course_files_by_course_async**](CoursesApi.md#get_course_files_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Files | Get course files by course
[**get_course_files_by_course_count_async**](CoursesApi.md#get_course_files_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Files/Count | Get course files by course count
[**get_course_forums_by_course_async**](CoursesApi.md#get_course_forums_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Forums | Get course forums by course
[**get_course_forums_by_course_count_async**](CoursesApi.md#get_course_forums_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Forums/Count | Get course forums by course count
[**get_course_handouts_by_course_async**](CoursesApi.md#get_course_handouts_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Handouts | Get course handouts by course
[**get_course_handouts_by_course_count_async**](CoursesApi.md#get_course_handouts_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Handouts/Count | Get course handouts by course count
[**get_course_libraries_by_course_async**](CoursesApi.md#get_course_libraries_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Libraries | Get course libraries by course
[**get_course_libraries_by_course_count_async**](CoursesApi.md#get_course_libraries_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Libraries/Count | Get course libraries by course count
[**get_course_pages_by_course_async**](CoursesApi.md#get_course_pages_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Pages | Get course pages by course
[**get_course_pages_by_course_count_async**](CoursesApi.md#get_course_pages_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Pages/Count | Get course pages by course count
[**get_course_problem_sets_by_course_async**](CoursesApi.md#get_course_problem_sets_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ProblemSets | Get course problem sets by course
[**get_course_problem_sets_by_course_count_async**](CoursesApi.md#get_course_problem_sets_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ProblemSets/Count | Get course problem sets by course count
[**get_course_sections_by_course_async**](CoursesApi.md#get_course_sections_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Sections | Get course sections by course
[**get_course_sections_by_course_count_async**](CoursesApi.md#get_course_sections_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Sections/Count | Get course sections by course count
[**get_course_unit_components_by_course_async**](CoursesApi.md#get_course_unit_components_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/UnitComponents | Get course unit components by course
[**get_course_unit_components_by_course_count_async**](CoursesApi.md#get_course_unit_components_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/UnitComponents/Count | Get course unit components by course count
[**get_course_units_by_section_async**](CoursesApi.md#get_course_units_by_section_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Units/{sectionId} | Get course units by section
[**get_course_units_by_section_count_async**](CoursesApi.md#get_course_units_by_section_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Units/{sectionId}/Count | Get course units by section count
[**get_course_updates_by_course_async**](CoursesApi.md#get_course_updates_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Updates | Get course updates by course
[**get_course_updates_by_course_count_async**](CoursesApi.md#get_course_updates_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Updates/Count | Get course updates by course count
[**get_course_wikis_by_course_async**](CoursesApi.md#get_course_wikis_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Wikis | Get course wikis by course
[**get_course_wikis_by_course_count_async**](CoursesApi.md#get_course_wikis_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Wikis/Count | Get course wikis by course count
[**get_courses_async**](CoursesApi.md#get_courses_async) | **GET** /api/v2/LearningService/Courses | Get courses
[**get_courses_count_async**](CoursesApi.md#get_courses_count_async) | **GET** /api/v2/LearningService/Courses/Count | Get courses count
[**get_instructor_profiles_by_course_async**](CoursesApi.md#get_instructor_profiles_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Instructors | Get instructor profiles by course
[**get_instructor_profiles_by_course_count_async**](CoursesApi.md#get_instructor_profiles_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Instructors/Count | Get instructor profiles by course count
[**get_student_profiles_by_course_async**](CoursesApi.md#get_student_profiles_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Students | Get student profiles by course
[**get_student_profiles_by_course_count_async**](CoursesApi.md#get_student_profiles_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Students/Count | Get student profiles by course count
[**update_course_async**](CoursesApi.md#update_course_async) | **PUT** /api/v2/LearningService/Courses/{courseId} | Update a course



## create_course_async

> create_course_async(tenant_id, api_version, x_api_version, course_create_dto)
Create a new course

Creates a new course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_create_dto** | Option<[**CourseCreateDto**](CourseCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_async

> delete_course_async(tenant_id, course_id, api_version, x_api_version)
Delete a course

Deletes a course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
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


## get_course_articles_by_course_wiki_async

> Vec<models::CourseArticleDto> get_course_articles_by_course_wiki_async(course_id, wiki_id, api_version, x_api_version)
Get course articles by course wiki

Retrieves all course articles for a specific course wiki.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**wiki_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseArticleDto>**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_articles_by_course_wiki_count_async

> i32 get_course_articles_by_course_wiki_count_async(course_id, wiki_id, api_version, x_api_version)
Get course articles by course wiki count

Returns the count of course articles for a specific course wiki.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**wiki_id** | **String** |  | [required] |
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


## get_course_assignments_by_course_async

> Vec<models::CourseAssignmentDto> get_course_assignments_by_course_async(course_id, api_version, x_api_version)
Get course assignments by course

Retrieves all course assignments for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseAssignmentDto>**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_assignments_by_course_count_async

> i32 get_course_assignments_by_course_count_async(course_id, api_version, x_api_version)
Get course assignments by course count

Returns the count of course assignments for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_by_id_async

> models::CourseDto get_course_by_id_async(tenant_id, course_id, api_version, x_api_version)
Get course by ID

Retrieves a specific course by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseDto**](CourseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_categories_by_course_async

> Vec<models::CourseCategoryDto> get_course_categories_by_course_async(course_id, api_version, x_api_version)
Get course categories by course

Retrieves all course categories for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseCategoryDto>**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_categories_by_course_count_async

> i32 get_course_categories_by_course_count_async(course_id, api_version, x_api_version)
Get course categories by course count

Returns the count of course categories for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_cohorts_by_course_async

> Vec<models::CourseCohortDto> get_course_cohorts_by_course_async(course_id, api_version, x_api_version)
Get course cohorts by course

Retrieves all course cohorts for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseCohortDto>**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_cohorts_by_course_count_async

> i32 get_course_cohorts_by_course_count_async(course_id, api_version, x_api_version)
Get course cohorts by course count

Returns the count of course cohorts for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_enrollments_by_course_async

> Vec<models::CourseEnrollmentDto> get_course_enrollments_by_course_async(tenant_id, course_id, api_version, x_api_version)
Get enrollments by course

Retrieves all enrollments for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseEnrollmentDto>**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_files_by_course_async

> Vec<models::CourseFileDto> get_course_files_by_course_async(course_id, api_version, x_api_version)
Get course files by course

Retrieves all course files for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseFileDto>**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_files_by_course_count_async

> i32 get_course_files_by_course_count_async(course_id, api_version, x_api_version)
Get course files by course count

Returns the count of course files for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_forums_by_course_async

> Vec<models::CourseForumDto> get_course_forums_by_course_async(course_id, api_version, x_api_version)
Get course forums by course

Retrieves all course forums for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseForumDto>**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_forums_by_course_count_async

> i32 get_course_forums_by_course_count_async(course_id, api_version, x_api_version)
Get course forums by course count

Returns the count of course forums for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_handouts_by_course_async

> Vec<models::CourseHandoutDto> get_course_handouts_by_course_async(course_id, api_version, x_api_version)
Get course handouts by course

Retrieves all course handouts for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseHandoutDto>**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_handouts_by_course_count_async

> i32 get_course_handouts_by_course_count_async(course_id, api_version, x_api_version)
Get course handouts by course count

Returns the count of course handouts for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_libraries_by_course_async

> Vec<models::CourseLibraryDto> get_course_libraries_by_course_async(course_id, api_version, x_api_version)
Get course libraries by course

Retrieves all course libraries for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseLibraryDto>**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_libraries_by_course_count_async

> i32 get_course_libraries_by_course_count_async(course_id, api_version, x_api_version)
Get course libraries by course count

Returns the count of course libraries for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_pages_by_course_async

> Vec<models::CoursePageDto> get_course_pages_by_course_async(course_id, api_version, x_api_version)
Get course pages by course

Retrieves all course pages for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CoursePageDto>**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_pages_by_course_count_async

> i32 get_course_pages_by_course_count_async(course_id, api_version, x_api_version)
Get course pages by course count

Returns the count of course pages for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_problem_sets_by_course_async

> Vec<models::CourseProblemSetDto> get_course_problem_sets_by_course_async(course_id, api_version, x_api_version)
Get course problem sets by course

Retrieves all course problem sets for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseProblemSetDto>**](CourseProblemSetDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_problem_sets_by_course_count_async

> i32 get_course_problem_sets_by_course_count_async(course_id, api_version, x_api_version)
Get course problem sets by course count

Returns the count of course problem sets for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_sections_by_course_async

> Vec<models::CourseSectionDto> get_course_sections_by_course_async(course_id, api_version, x_api_version)
Get course sections by course

Retrieves all course sections for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseSectionDto>**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_sections_by_course_count_async

> i32 get_course_sections_by_course_count_async(course_id, api_version, x_api_version)
Get course sections by course count

Returns the count of course sections for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_unit_components_by_course_async

> Vec<models::CourseUnitComponentDto> get_course_unit_components_by_course_async(course_id, api_version, x_api_version)
Get course unit components by course

Retrieves all course unit components for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseUnitComponentDto>**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_unit_components_by_course_count_async

> i32 get_course_unit_components_by_course_count_async(course_id, api_version, x_api_version)
Get course unit components by course count

Returns the count of course unit components for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_units_by_section_async

> Vec<models::CourseUnitDto> get_course_units_by_section_async(course_id, section_id, api_version, x_api_version)
Get course units by section

Retrieves all course units for a specific course section.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**section_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseUnitDto>**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_units_by_section_count_async

> i32 get_course_units_by_section_count_async(course_id, section_id, api_version, x_api_version)
Get course units by section count

Returns the count of course units for a specific course section.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**section_id** | **String** |  | [required] |
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


## get_course_updates_by_course_async

> Vec<models::CourseNewsDto> get_course_updates_by_course_async(course_id, api_version, x_api_version)
Get course updates by course

Retrieves all course updates for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseNewsDto>**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_updates_by_course_count_async

> i32 get_course_updates_by_course_count_async(course_id, api_version, x_api_version)
Get course updates by course count

Returns the count of course updates for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_course_wikis_by_course_async

> Vec<models::CourseWikiDto> get_course_wikis_by_course_async(course_id, api_version, x_api_version)
Get course wikis by course

Retrieves all course wikis for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseWikiDto>**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_wikis_by_course_count_async

> i32 get_course_wikis_by_course_count_async(course_id, api_version, x_api_version)
Get course wikis by course count

Returns the count of course wikis for a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_courses_async

> Vec<models::CourseDto> get_courses_async(tenant_id, api_version, x_api_version)
Get courses

Retrieves courses. When tenantId is provided, returns tenant-scoped courses; otherwise returns all courses.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseDto>**](CourseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_courses_count_async

> i32 get_courses_count_async(tenant_id, api_version, x_api_version)
Get courses count

Returns the count of courses. When tenantId is provided, returns tenant-scoped count; otherwise returns global count.

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


## get_instructor_profiles_by_course_async

> Vec<models::InstructorProfileDto> get_instructor_profiles_by_course_async(course_id, api_version, x_api_version)
Get instructor profiles by course

Retrieves all instructor profiles teaching a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::InstructorProfileDto>**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_instructor_profiles_by_course_count_async

> i32 get_instructor_profiles_by_course_count_async(course_id, api_version, x_api_version)
Get instructor profiles by course count

Returns the count of instructor profiles teaching a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## get_student_profiles_by_course_async

> Vec<models::StudentProfileDto> get_student_profiles_by_course_async(course_id, api_version, x_api_version)
Get student profiles by course

Retrieves all student profiles enrolled in a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::StudentProfileDto>**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_student_profiles_by_course_count_async

> i32 get_student_profiles_by_course_count_async(course_id, api_version, x_api_version)
Get student profiles by course count

Returns the count of student profiles enrolled in a specific course.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**course_id** | **String** |  | [required] |
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


## update_course_async

> update_course_async(tenant_id, course_id, api_version, x_api_version, course_update_dto)
Update a course

Updates an existing course for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_update_dto** | Option<[**CourseUpdateDto**](CourseUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

