# \CognitiveAgentConversationAttachmentsApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**upload_cognitive_agent_conversation_attachment_async**](CognitiveAgentConversationAttachmentsApi.md#upload_cognitive_agent_conversation_attachment_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Attachments | Upload an attachment to a cognitive agent conversation



## upload_cognitive_agent_conversation_attachment_async

> models::ConversationAttachmentUploadResultDtoEnvelope upload_cognitive_agent_conversation_attachment_async(tenant_id, agent_id, conversation_id, api_version, x_api_version, file)
Upload an attachment to a cognitive agent conversation

Uploads a file into the acting user's OWN conversation attachment store, scanned and catalogued through the storage spine. A conversation the caller does not own returns 404. The response carries the new file's id, name, content type and length; the chat UI passes that id as an AttachmentFileIds entry when it sends the referencing user turn.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tenant_id** | **uuid::Uuid** |  | [required] |
**agent_id** | **uuid::Uuid** |  | [required] |
**conversation_id** | **uuid::Uuid** |  | [required] |
**api_version** | Option<**String**> |  |  |
**x_api_version** | Option<**String**> |  |  |
**file** | Option<**std::path::PathBuf**> |  |  |

### Return type

[**models::ConversationAttachmentUploadResultDtoEnvelope**](ConversationAttachmentUploadResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

