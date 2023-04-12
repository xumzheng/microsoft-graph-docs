---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcProvisioningPolicy()
request_body.@odatatype = '#microsoft.graph.cloudPcProvisioningPolicy'

request_body.displayName = 'HR provisioning policy'

request_body.description = 'Provisioning policy for India HR employees'

request_body.onPremisesConnectionId = '4e47d0f6-6f77-44f0-8893-c0fe1701ffff'

request_body.imageId = 'Image ID value'

request_body.imageDisplayName = 'Image Display Name value'

request_body.ImageType(CloudPcProvisioningPolicyImageType('custom'))

windowsSettings = CloudPcWindowsSettings()
windowsSettings.language = 'en-US'


request_body.windowsSettings = windowsSettings



result = await client.deviceManagement.virtualEndpoint.provisioningPolicies_by_id('cloudPcProvisioningPolicy-id').patch(request_body = request_body)


```