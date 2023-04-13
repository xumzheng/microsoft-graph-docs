---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcProvisioningPolicy()
request_body.@odatatype = '#microsoft.graph.cloudPcProvisioningPolicy'

request_body.description = 'Description value'

request_body.displayName = 'Display Name value'

domain_join_configuration = CloudPcDomainJoinConfiguration()
domainJoinConfiguration.onPremisesConnectionId = '16ee6c71-fc10-438b-88ac-daa1ccafffff'

additionalData = [
'domainJoinType' => 'hybridAzureADJoin', 
];
domainJoinConfiguration.additionaldata(additionalData)



request_body.domain_join_configuration = domainJoinConfiguration
request_body.enable_single_sign_on = True

request_body.imageDisplayName = 'Windows-10 19h1-evd'

request_body.imageId = 'MicrosoftWindowsDesktop_Windows-10_19h1-evd'

request_body.ImageType(CloudPcProvisioningPolicyImageType('gallery'))

request_body.onPremisesConnectionId = '4e47d0f6-6f77-44f0-8893-c0fe1701ffff'

windows_settings = CloudPcWindowsSettings()
windowsSettings.language = 'en-US'


request_body.windows_settings = windowsSettings
request_body.ProvisioningType(CloudPcProvisioningType('dedicated'))




result = await client.deviceManagement.virtualEndpoint.provisioningPolicies.post(request_body = request_body)


```