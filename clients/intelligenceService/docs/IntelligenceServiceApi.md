# \IntelligenceServiceApi

All URIs are relative to *https://absuite.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**invoke_agent_surface_async**](IntelligenceServiceApi.md#invoke_agent_surface_async) | **POST** /api/v2/IntelligenceService/Agents/{agentId}/agui | Run a governed agent over the AG-UI protocol



## invoke_agent_surface_async

> invoke_agent_surface_async(agent_id)
Run a governed agent over the AG-UI protocol

Streams a governed agent run as AG-UI server-sent events. Feature-flagged on ABP.Cognitive.AgentSurface.Enable; returns 503 when disabled, 401 when unauthorized and 404 when the agent cannot be resolved. An optional ?projectId= binds the run to a project (resolved tenant-scoped): the project id + name are surfaced to the model as context so it can call the governed project-storage tools; it is never auto-filled into a tool's arguments.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**agent_id** | **String** |  | [required] |

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

