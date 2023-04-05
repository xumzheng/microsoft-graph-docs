---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcProvisioningPolicy()
request_body.set@odatatype('#microsoft.graph.cloudPcProvisioningPolicy')

request_body.setDisplayName('HR provisioning policy')

request_body.setDescription('Provisioning policy for India HR employees')

request_body.setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff')

request_body.setImageId('Image ID value')

request_body.setImageDisplayName('Image Display Name value')

request_body.setImageType(CloudPcProvisioningPolicyImageType('custom'))

windowsSettings = CloudPcWindowsSettings()
windowsSettings.setLanguage('en-US')


request_body.setWindowsSettings($windowsSettings)


result = await client.deviceManagement_virtualEndpoint_provisioningPoliciesby_id('cloudPcProvisioningPolicy-id').patch(request_body)


```