# ExecutionContext

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_authenticated** | Option<**bool**> |  | [optional]
**current_cart_id** | Option<**String**> |  | [optional][readonly]
**current_user_id** | Option<**String**> |  | [optional][readonly]
**current_tenant_id** | Option<**String**> |  | [optional][readonly]
**current_portal_id** | Option<**String**> |  | [optional][readonly]
**current_enrollment_id** | Option<**String**> |  | [optional][readonly]
**currency_id** | Option<**String**> |  | [optional][readonly]
**page_size** | Option<**i32**> |  | [optional]
**date_format** | Option<**String**> |  | [optional]
**currency_format** | Option<**String**> |  | [optional]
**date_time_format** | Option<**String**> |  | [optional]
**to_date_data_summaries** | Option<**String**> |  | [optional]
**from_date_data_summaries** | Option<**String**> |  | [optional]
**authorization** | Option<[**models::AuthResult**](AuthResult.md)> |  | [optional]
**user** | Option<[**models::ExtendedUserDto**](ExtendedUserDto.md)> |  | [optional]
**current_tenant** | Option<[**models::ExtendedTenantDto**](ExtendedTenantDto.md)> |  | [optional]
**current_enrollment** | Option<[**models::TenantEnrollmentDto**](TenantEnrollmentDto.md)> |  | [optional]
**selected_tenant_mappings** | Option<[**models::CrmContext**](CrmContext.md)> |  | [optional]
**portal_owner_mappings** | Option<[**models::CrmContext**](CrmContext.md)> |  | [optional]
**root_tenant_mappings** | Option<[**models::CrmContext**](CrmContext.md)> |  | [optional]
**cart** | Option<[**models::CartDto**](CartDto.md)> |  | [optional]
**currency** | Option<[**models::CurrencyDto**](CurrencyDto.md)> |  | [optional]
**forex_rates** | Option<[**models::ForexRatesDto**](ForexRatesDto.md)> |  | [optional]
**exchange_rate** | Option<[**models::Money**](Money.md)> |  | [optional]
**country** | Option<[**models::CountryDto**](CountryDto.md)> |  | [optional]
**root_tenant** | Option<[**models::TenantDto**](TenantDto.md)> |  | [optional]
**current_portal** | Option<[**models::WebPortalDto**](WebPortalDto.md)> |  | [optional]
**tenants** | Option<[**Vec<models::ExtendedTenantDto>**](ExtendedTenantDto.md)> |  | [optional]
**enrollments** | Option<[**Vec<models::ExtendedTenantEnrollmentDto>**](ExtendedTenantEnrollmentDto.md)> |  | [optional]
**available_portals** | Option<[**Vec<models::WebPortalDto>**](WebPortalDto.md)> |  | [optional]
**invitations** | Option<[**Vec<models::ExtendedInviteDto>**](ExtendedInviteDto.md)> |  | [optional]
**granted_permissions** | Option<**Vec<String>**> |  | [optional]
**accessible_features** | Option<[**Vec<models::SuiteLicenseFeatureDto>**](SuiteLicenseFeatureDto.md)> |  | [optional]
**culture_name** | Option<**String**> |  | [optional][readonly]
**timezone_id** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


