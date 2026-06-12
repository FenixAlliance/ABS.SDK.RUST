# ClaimsIdentity

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authentication_type** | Option<**String**> |  | [optional][readonly]
**is_authenticated** | Option<**bool**> |  | [optional][readonly]
**actor** | Option<[**models::ClaimsIdentity**](ClaimsIdentity.md)> |  | [optional]
**bootstrap_context** | Option<[**serde_json::Value**](.md)> |  | [optional]
**claims** | Option<[**Vec<models::Claim>**](Claim.md)> |  | [optional][readonly]
**label** | Option<**String**> |  | [optional]
**name** | Option<**String**> |  | [optional][readonly]
**name_claim_type** | Option<**String**> |  | [optional][readonly]
**role_claim_type** | Option<**String**> |  | [optional][readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


