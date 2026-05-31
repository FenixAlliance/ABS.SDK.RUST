# LicenseKeyRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**tenant_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**order_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**payment_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**invoice_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**enrollment_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**entitlement_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> |  | [optional]
**seats** | Option<**i32**> |  | [optional]
**license_type** | Option<**String**> |  | [optional]
**expiration_date** | Option<**String**> |  | [optional]
**features** | Option<[**Vec<models::LicenseFeature>**](LicenseFeature.md)> |  | [optional]
**additional_attributes** | Option<[**Vec<models::AdditionalAttribute>**](AdditionalAttribute.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


