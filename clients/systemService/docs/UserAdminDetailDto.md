# UserAdminDetailDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orders** | Option<[**Vec<models::UserOrderSummaryDto>**](UserOrderSummaryDto.md)> |  | [optional]
**logins** | Option<[**Vec<models::UserExternalLoginDto>**](UserExternalLoginDto.md)> |  | [optional]
**enrollment** | Option<[**models::TenantEnrollmentDto**](TenantEnrollmentDto.md)> |  | [optional]
**granted_roles** | Option<[**Vec<models::SecurityRoleDto>**](SecurityRoleDto.md)> |  | [optional]
**granted_permissions** | Option<[**Vec<models::SecurityPermissionDto>**](SecurityPermissionDto.md)> |  | [optional]
**role_catalog** | Option<[**Vec<models::SecurityRoleDto>**](SecurityRoleDto.md)> |  | [optional]
**permission_catalog** | Option<[**Vec<models::SecurityPermissionDto>**](SecurityPermissionDto.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


