# Event

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreationTime** | **string** | Read-only | [optional] [default to null]
**EventType** | **string** | Type of event, consumer cannot set recommend | [optional] [default to null]
**EventId** | **string** | Read-only | [optional] [default to null]
**EventTime** | **string** | Read-only | [optional] [default to null]
**EntityType** | **string** | Read-only | [optional] [default to null]
**EntityId** | **string** | The user that triggered this event. You are free to choose whatever you like but it has to be consistent. Good examples are email address, internal user id or sha256 hash of these values. | [optional] [default to null]
**TargetEntityType** | **string** | Read-only | [optional] [default to null]
**TargetEntityId** | **string** | Way to identify your product. Use the product id from your shop | [optional] [default to null]
**Body** | **string** | Meta information that doesn&#39;t fit into above fields. Read-only | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


