---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CloudPcProvisioningPolicy()
request_body.set@odatatype('#microsoft.graph.cloudPcProvisioningPolicy')

request_body.setDescription('Description value')

request_body.setDisplayName('Display Name value')

domainJoinConfiguration = CloudPcDomainJoinConfiguration()
domainJoinConfiguration.setOnPremisesConnectionId('16ee6c71-fc10-438b-88ac-daa1ccafffff')

additionalData = [
'domainJoinType' => 'hybridAzureADJoin', 
];
domainJoinConfiguration.setAdditionalData(additionalData)



request_body.setDomainJoinConfiguration($domainJoinConfiguration)
request_body.setEnableSingleSignOn(true)

request_body.setImageDisplayName('Windows-10 19h1-evd')

request_body.setImageId('MicrosoftWindowsDesktop_Windows-10_19h1-evd')

request_body.setImageType(CloudPcProvisioningPolicyImageType('gallery'))

request_body.setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff')

windowsSettings = CloudPcWindowsSettings()
windowsSettings.setLanguage('en-US')


request_body.setWindowsSettings($windowsSettings)
request_body.setProvisioningType(CloudPcProvisioningType('dedicated'))



result = await client.deviceManagement.virtualEndpoint.provisioningPolicies.post(request_body)


```