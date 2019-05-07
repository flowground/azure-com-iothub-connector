# ![LOGO](logo.png) iotHubClient **flow**ground Connector

## Description

A generated **flow**ground connector for the iotHubClient API (version 2018-12-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/iothub/2018-12-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:38:14+03:00

## API Description

Use this API to manage the IoT hubs in your Azure subscription.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the available IoT Hub REST API operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - The version of the API.

### Get all the IoT hubs in a subscription

> Get all the IoT hubs in a subscription.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.

### Check if an IoT hub name is available

> Check if an IoT hub name is available.

*Tags:* `POST`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.

### Get the number of iot hubs in the subscription

> Get the number of free and paid iot hubs in the subscription

*Tags:* `GET`

#### Input Parameters
* `subscriptionId` - _required_ - The subscription identifier.
* `api-version` - _required_ - The version of the API.

### Get all the IoT hubs in a resource group

> Get all the IoT hubs in a resource group.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.

### Test all routes

> Test all routes configured in this Iot Hub

*Tags:* `POST`

#### Input Parameters
* `iotHubName` - _required_ - IotHub to be tested
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - resource group which Iot Hub belongs to
* `api-version` - _required_ - The version of the API.

### Test the new route

> Test the new route for this Iot Hub

*Tags:* `POST`

#### Input Parameters
* `iotHubName` - _required_ - IotHub to be tested
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - resource group which Iot Hub belongs to
* `api-version` - _required_ - The version of the API.

### Get the health for routing endpoints

> Get the health for routing endpoints.

*Tags:* `GET`

#### Input Parameters
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_
* `iotHubName` - _required_
* `api-version` - _required_ - The version of the API.

### Delete an IoT hub

> Delete an IoT hub.

*Tags:* `DELETE`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get the non-security related metadata of an IoT hub

> Get the non-security related metadata of an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Update an existing IoT Hubs tags.

> Update an existing IoT Hub tags. to update other fields use the CreateOrUpdate method

*Tags:* `PATCH`

#### Input Parameters
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - Resource group identifier.
* `resourceName` - _required_ - Name of iot hub to update.
* `api-version` - _required_ - The version of the API.

### Create or update the metadata of an IoT hub.

> Create or update the metadata of an Iot hub. The usual pattern to modify a property is to retrieve the IoT hub metadata and security metadata, and then combine them with the modified values in a new body to update the IoT hub.

*Tags:* `PUT`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `If-Match` - _optional_ - ETag of the IoT Hub. Do not specify for creating a brand new IoT Hub. Required to update an existing IoT Hub.

### Get a shared access policy by name from an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-security

> Get a shared access policy by name from an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-security.

*Tags:* `POST`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `keyName` - _required_ - The name of the shared access policy.

### Get the statistics from an IoT hub

> Get the statistics from an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get the certificate list.

> Returns the list of certificates.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Delete an X509 certificate.

> Deletes an existing X509 certificate or does nothing if it does not exist.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `certificateName` - _required_ - The name of the certificate
* `If-Match` - _required_ - ETag of the Certificate.

### Get the certificate.

> Returns the certificate.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `certificateName` - _required_ - The name of the certificate

### Upload the certificate to the IoT hub.

> Adds new or replaces existing certificate.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `certificateName` - _required_ - The name of the certificate
* `If-Match` - _optional_ - ETag of the Certificate. Do not specify for creating a brand new certificate. Required to update an existing certificate.

### Generate verification code for proof of possession flow.

> Generates verification code for proof of possession flow. The verification code will be used to generate a leaf certificate.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `certificateName` - _required_ - The name of the certificate
* `If-Match` - _required_ - ETag of the Certificate.

### Verify certificate's private key possession.

> Verifies the certificate's private key possession by providing the leaf cert issued by the verifying pre uploaded certificate.

*Tags:* `Certificates`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `certificateName` - _required_ - The name of the certificate
* `If-Match` - _required_ - ETag of the Certificate.

### Get a list of the consumer groups in the Event Hub-compatible device-to-cloud endpoint in an IoT hub

> Get a list of the consumer groups in the Event Hub-compatible device-to-cloud endpoint in an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `eventHubEndpointName` - _required_ - The name of the Event Hub-compatible endpoint.

### Delete a consumer group from an Event Hub-compatible endpoint in an IoT hub

> Delete a consumer group from an Event Hub-compatible endpoint in an IoT hub.

*Tags:* `DELETE`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `eventHubEndpointName` - _required_ - The name of the Event Hub-compatible endpoint in the IoT hub.
* `name` - _required_ - The name of the consumer group to delete.

### Get a consumer group from the Event Hub-compatible device-to-cloud endpoint for an IoT hub

> Get a consumer group from the Event Hub-compatible device-to-cloud endpoint for an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `eventHubEndpointName` - _required_ - The name of the Event Hub-compatible endpoint in the IoT hub.
* `name` - _required_ - The name of the consumer group to retrieve.

### Add a consumer group to an Event Hub-compatible endpoint in an IoT hub

> Add a consumer group to an Event Hub-compatible endpoint in an IoT hub.

*Tags:* `PUT`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `eventHubEndpointName` - _required_ - The name of the Event Hub-compatible endpoint in the IoT hub.
* `name` - _required_ - The name of the consumer group to add.

### Exports all the device identities in the IoT hub identity registry to an Azure Storage blob container. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities

> Exports all the device identities in the IoT hub identity registry to an Azure Storage blob container. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.

*Tags:* `POST`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Import, update, or delete device identities in the IoT hub identity registry from a blob. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities

> Import, update, or delete device identities in the IoT hub identity registry from a blob. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry#import-and-export-device-identities.

*Tags:* `POST`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get a list of all the jobs in an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry

> Get a list of all the jobs in an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get the details of a job from an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry

> Get the details of a job from an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-identity-registry.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.
* `jobId` - _required_ - The job identifier.

### Get the security metadata for an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-security

> Get the security metadata for an IoT hub. For more information, see: https://docs.microsoft.com/azure/iot-hub/iot-hub-devguide-security.

*Tags:* `POST`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get the quota metrics for an IoT hub

> Get the quota metrics for an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

### Get the list of valid SKUs for an IoT hub

> Get the list of valid SKUs for an IoT hub.

*Tags:* `GET`

#### Input Parameters
* `api-version` - _required_ - The version of the API.
* `subscriptionId` - _required_ - The subscription identifier.
* `resourceGroupName` - _required_ - The name of the resource group that contains the IoT hub.
* `resourceName` - _required_ - The name of the IoT hub.

## License

**flow**ground :- Telekom iPaaS / azure-com-iothub-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
