# \CourseCertificatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_course_certificate_async**](CourseCertificatesApi.md#create_course_certificate_async) | **POST** /api/v2/LearningService/CourseCertificates | Create a course certificate
[**create_course_certificate_template_async**](CourseCertificatesApi.md#create_course_certificate_template_async) | **POST** /api/v2/LearningService/CourseCertificates/Template | Create a certificate template
[**delete_course_certificate_async**](CourseCertificatesApi.md#delete_course_certificate_async) | **DELETE** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Delete a course certificate
[**delete_course_certificate_template_async**](CourseCertificatesApi.md#delete_course_certificate_template_async) | **DELETE** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Delete a certificate template
[**get_course_certificate_async**](CourseCertificatesApi.md#get_course_certificate_async) | **GET** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Get course certificate by ID
[**get_course_certificate_template_async**](CourseCertificatesApi.md#get_course_certificate_template_async) | **GET** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Get certificate template by ID
[**get_course_certificate_templates_async**](CourseCertificatesApi.md#get_course_certificate_templates_async) | **GET** /api/v2/LearningService/CourseCertificates/Template | Get all certificate templates
[**get_course_certificates_async**](CourseCertificatesApi.md#get_course_certificates_async) | **GET** /api/v2/LearningService/CourseCertificates | Get all course certificates
[**get_course_certificates_count_async**](CourseCertificatesApi.md#get_course_certificates_count_async) | **GET** /api/v2/LearningService/CourseCertificates/Count | Get course certificates count
[**update_course_certificate_async**](CourseCertificatesApi.md#update_course_certificate_async) | **PUT** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Update a course certificate



## create_course_certificate_async

> create_course_certificate_async(tenant_id, api_version, x_api_version, course_completion_certificate_create_dto)
Create a course certificate

Creates a new course certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_completion_certificate_create_dto** | Option<[**CourseCompletionCertificateCreateDto**](CourseCompletionCertificateCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_course_certificate_template_async

> create_course_certificate_template_async(tenant_id, api_version, x_api_version, course_certificate_template_create_dto)
Create a certificate template

Creates a new course certificate template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_certificate_template_create_dto** | Option<[**CourseCertificateTemplateCreateDto**](CourseCertificateTemplateCreateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_course_certificate_async

> delete_course_certificate_async(tenant_id, course_certificate_id, api_version, x_api_version)
Delete a course certificate

Deletes a course certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_certificate_id** | **uuid::Uuid** |  | [required] |
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


## delete_course_certificate_template_async

> delete_course_certificate_template_async(tenant_id, course_certificate_template_id, api_version, x_api_version)
Delete a certificate template

Deletes a course certificate template for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_certificate_template_id** | **uuid::Uuid** |  | [required] |
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


## get_course_certificate_async

> models::CourseCompletionCertificateDto get_course_certificate_async(tenant_id, course_certificate_id, api_version, x_api_version)
Get course certificate by ID

Retrieves a specific course certificate by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_certificate_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseCompletionCertificateDto**](CourseCompletionCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_certificate_template_async

> models::CourseCertificateTemplateDto get_course_certificate_template_async(tenant_id, course_certificate_template_id, api_version, x_api_version)
Get certificate template by ID

Retrieves a specific course certificate template by its ID.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_certificate_template_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**models::CourseCertificateTemplateDto**](CourseCertificateTemplateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_certificate_templates_async

> Vec<models::CourseCertificateTemplateDto> get_course_certificate_templates_async(tenant_id, api_version, x_api_version)
Get all certificate templates

Retrieves all course certificate templates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseCertificateTemplateDto>**](CourseCertificateTemplateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_certificates_async

> Vec<models::CourseCompletionCertificateDto> get_course_certificates_async(tenant_id, api_version, x_api_version)
Get all course certificates

Retrieves all course certificates for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |

### Return type

[**Vec<models::CourseCompletionCertificateDto>**](CourseCompletionCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_course_certificates_count_async

> i32 get_course_certificates_count_async(tenant_id, api_version, x_api_version)
Get course certificates count

Returns the count of course certificates for the specified tenant.

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


## update_course_certificate_async

> update_course_certificate_async(tenant_id, course_certificate_id, api_version, x_api_version, course_completion_certificate_update_dto)
Update a course certificate

Updates an existing course certificate for the specified tenant.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**course_certificate_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**course_completion_certificate_update_dto** | Option<[**CourseCompletionCertificateUpdateDto**](CourseCompletionCertificateUpdateDto.md)> |  |  |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

