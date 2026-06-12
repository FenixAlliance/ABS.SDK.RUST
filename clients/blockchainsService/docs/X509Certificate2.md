# X509Certificate2

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**handle** | Option<[**serde_json::Value**](.md)> |  | [optional]
**issuer** | Option<**String**> |  | [optional][readonly]
**subject** | Option<**String**> |  | [optional][readonly]
**serial_number_bytes** | Option<[**models::ByteReadOnlyMemory**](ByteReadOnlyMemory.md)> |  | [optional]
**archived** | Option<**bool**> |  | [optional]
**extensions** | Option<[**Vec<models::X509Extension>**](X509Extension.md)> |  | [optional][readonly]
**friendly_name** | Option<**String**> |  | [optional]
**has_private_key** | Option<**bool**> |  | [optional][readonly]
**private_key** | Option<[**models::AsymmetricAlgorithm**](AsymmetricAlgorithm.md)> |  | [optional]
**issuer_name** | Option<[**models::X500DistinguishedName**](X500DistinguishedName.md)> |  | [optional]
**not_after** | Option<**String**> |  | [optional][readonly]
**not_before** | Option<**String**> |  | [optional][readonly]
**public_key** | Option<[**models::PublicKey**](PublicKey.md)> |  | [optional]
**raw_data** | Option<**String**> |  | [optional][readonly]
**raw_data_memory** | Option<[**models::ByteReadOnlyMemory**](ByteReadOnlyMemory.md)> |  | [optional]
**serial_number** | Option<**String**> |  | [optional][readonly]
**signature_algorithm** | Option<[**models::Oid**](Oid.md)> |  | [optional]
**subject_name** | Option<[**models::X500DistinguishedName**](X500DistinguishedName.md)> |  | [optional]
**thumbprint** | Option<**String**> |  | [optional][readonly]
**version** | Option<**i32**> |  | [optional][readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


